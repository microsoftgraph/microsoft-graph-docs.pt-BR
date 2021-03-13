---
title: Diferenças de recursos entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças de recursos entre a API do Azure Active Directory (Azure AD) e a API do Microsoft Graph, para ajudar você a migrar aplicativos de forma rápida e fácil.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: a404c69370c7b6aaeee07e20df1165c43a98a243
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760676"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de recursos entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: analisar as* diferenças de API do processo para [migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Muitos recursos no Microsoft Graph funcionam da mesma forma que seus equivalentes do Azure AD Graph. No entanto, alguns foram alterados e/ou melhorados. Aqui, você aprenderá a adaptar seus aplicativos para tirar proveito dessas diferenças.  Frequentemente, as alterações são secundárias, mas vale a pena o esforço.

Este artigo explora como o Microsoft Graph lida:

- Extensões de esquema de diretório
- Consultas diferenciais
- Envio em lote

## <a name="directory-schema-extensions"></a>Extensões de esquema de diretório

Se seu aplicativo usar extensões de diretório do Azure AD Graph, você poderá continuar a usar as mesmas APIs básicas (com URLs de solicitação do Microsoft Graph) para:

- Gerenciar definições de propriedade de extensão usando a propriedade **extensionProperties** no recurso [application][/graph/api/resources/application?view=graph-rest-v1.0).
- Obter propriedades de extensão disponíveis usando [a ação getAvailableExtensionProperties.](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-v1.0)
- Ler valores de extensão usando GET e `$select`
- Pesquisar valores de extensão usando GET e `$filter`
- Atualizar valores de extensão usando PATCH
- Remover valores de extensão usando PATCH (definido como **nulo**)

O Microsoft Graph fornece uma experiência de desenvolvedor de extensões de esquema aprimoradas, que hoje não é compatível com as extensões de diretório do Azure AD Graph. Para saber mais, confira [extensões de esquema em adicionar dados personalizados](./extensibility-overview.md#schema-extensions).

### <a name="recommended-migration-approach"></a>Abordagem de migração recomendada

Se o aplicativo do Azure AD Graph usar extensões de diretório, use uma abordagem incremental para migrar o aplicativo para o Microsoft Graph.

Primeiro, alternar seu aplicativo para usar chamadas de API do Microsoft Graph, mas permitir que o aplicativo continue a utilizar extensões de diretório do Azure AD Graph.

Em seguida, você pode alternar para usar extensões de esquema do Microsoft Graph. Em alguns casos, a alternação não será apropriada. Não alternar se:

- Seu aplicativo usa extensões de diretório criadas por meio do AD Connect
- Seu aplicativo define valores de extensão de diretório usados em declarações de token por outros aplicativos
- Seu aplicativo define valores de extensão de diretório usados em regras de associação dinâmicas 

>**OBSERVAÇÃO**: Ainda não há suporte para o uso das propriedades de extensão de esquema do Microsoft Graph como declarações em um token usando declarações opcionais ou em uma regra de associação dinâmica.

Para mudar para o modelo de extensão de esquema mais novo do Microsoft Graph, você precisará:

- Defina novas definições de extensão de esquema usando o Microsoft Graph.
- Atualize o aplicativo para dar suporte às novas definições de extensão de esquema.
- Migre os dados das propriedades de extensão do esquema do Azure AD para as novas propriedades de extensão de esquema do Microsoft Graph.  Não há suporte para migração automática de dados.

## <a name="differential-queries"></a>Consultas diferenciais

O Azure AD Graph e o Microsoft Graph permitem que você acompanhe as alterações usando consultas.  A abordagem de alto nível é semelhante entre as duas APIs, mas a sintaxe é diferente.

O Azure AD Graph chama essas consultas diferenciais.  No Microsoft Graph, elas são consultas [delta.](./delta-query-overview.md)

A tabela a seguir destaca as principais semelhanças e diferenças:

|Solicitação Delta |Azure AD Graph. | Microsoft Graph |
|----|----|----|
| _Solicitação de dados iniciais_ | Usa um parâmetro de consulta:<br>`GET /groups?deltaLink=` | Usa uma função: <br> `GET /groups/delta` |
| _Obter novas alterações_ | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| _Sincronizar a partir de agora_ |Usa um cabeçalho HTTP personalizado:<br> `ocp-aad-dq-include-only-delta-token: true` | Usa um parâmetro de consulta: <br> `GET /groups/delta?$deltaToken=latest` |
| _Rastrear alterações para directoryObjects_ | Obtém alterações para vários recursos (usuário e grupo) na mesma operação:&nbsp;&nbsp;<br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | Usa consultas separadas com o Microsoft Graph, uma para cada recurso. |
| _Obter alterações de recursos e relações_ | Todas as solicitações retornam alterações de recursos e relações, se o recurso tiver relações. | `GET /groups/delta?$expand=members` |
| _Resposta indicando itens novos e alterados_ | <ul><li><p>Representa instâncias recém-criadas usando sua representação padrão.</p></li><li><p>As instâncias atualizadas são representadas por sua id com pelo *menos* as propriedades que foram atualizadas. Outras propriedades podem ser incluídas.</p></li><li><p>As relações são representadas como o `directoryLinkChange` tipo.</p></li></ul>|<ul><li><p>Representa instâncias recém-criadas usando sua representação padrão.</p></li><li><p>As instâncias atualizadas são representadas por sua id com pelo *menos* as propriedades que foram atualizadas. Outras propriedades podem ser incluídas.</p></li><li><p>As relações são representadas como anotações na representação de recursos padrão. Essas anotações usam o formato `propertyName@delta` , por exemplo, `members@delta` para as alterações de associação de um grupo.</p></li></ul> |
| _Resposta indicando itens excluídos_| Indica um item excluído com uma propriedade adicional de *aad.isDeleted* definida como true. | Indica um item excluído com a \@ anotação removida. Também pode conter um código de motivo, que indica se o item foi excluído, mas pode ser restaurado ou excluído permanentemente. |

Se seu aplicativo já estiver armazenar dados de estado, considere usar a "sincronização a partir de agora" mostrada anteriormente para ajudar a gerenciar a transição para consultas delta.

## <a name="batching"></a>Envio em lote

O Azure AD Graph usou um sistema chamado mensagens MIME de várias partes para gerenciar o lote.  O Microsoft Graph usa [o lote JSON](json-batching.md) para permitir até 20 solicitações em uma única operação em lotes. O mecanismo de lote JSON é significativamente mais simples de usar, especialmente junto com bibliotecas de análise JSON.  Também permite sequenciar operações em lotes.  No entanto, ele não é compatível com a abordagem de lote do Azure AD Graph.

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre as diferenças de recursos](migrate-azure-ad-graph-resource-differences.md) entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->