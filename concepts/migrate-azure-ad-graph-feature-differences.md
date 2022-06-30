---
title: Diferenças de recursos entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças de recursos entre o Azure Active Directory (Azure AD) API do Graph e o Microsoft API do Graph, para ajudá-lo a migrar aplicativos de forma rápida e fácil.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 4ed6de06843d33c80dfcab28c885b7242ceede29
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555741"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de recursos entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: examinar as diferenças de API* do [processo para migrar aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Muitos recursos no Microsoft Graph funcionam da mesma forma que seus equivalentes do Graph do Azure Active Directory (Azure AD). No entanto, alguns foram alterados ou aprimorados. Aqui, você aprenderá a adaptar seus aplicativos para aproveitar essas diferenças.  Frequentemente, as alterações são pequenas, mas vale a pena o esforço.

Este artigo explora como o Microsoft Graph lida com:

- Extensões de esquema de diretório
- Consultas diferenciais
- Envio em lote

## <a name="directory-extensions"></a>Extensões de diretório

Se seu aplicativo usar Azure AD de diretório do Graph, você poderá continuar a usar as mesmas APIs básicas (com URLs de solicitação do Microsoft Graph) para:

- Gerencie definições de extensão de diretório usando [o recurso extensionProperty](/graph/api/resources/extensionproperty) e os métodos associados.
- Obtenha as propriedades de extensão disponíveis usando [a ação getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties) .
- Ler valores de extensão usando GET e para usuários, somente com `$select` uma consulta por meio do ponto `v1.0` de extremidade
- Pesquisar valores de extensão usando GET e `$filter`
- Atualizar valores de extensão usando PATCH
- Remover valores de extensão usando PATCH (definido como **nulo**)

O Microsoft Graph fornece uma experiência avançada de desenvolvedor de extensões de esquema, que hoje não é compatível com versões anteriores com Azure AD de diretório do Graph. Para saber mais, confira [Escolher um tipo de extensão para seu aplicativo](extensibility-overview.md#choose-an-extension-type-for-your-application).

### <a name="recommended-migration-approach"></a>Abordagem de migração recomendada

Se o Azure AD do Graph usar extensões de diretório, use uma abordagem incremental para migrar o aplicativo para o Microsoft Graph.

Primeiro, alterne seu aplicativo para usar chamadas do Microsoft API do Graph, mas permita que o aplicativo continue a aproveitar Azure AD de diretório do Graph.

Em seguida, você pode mudar para usar extensões de esquema do Microsoft Graph. Em alguns casos, a alternância não será apropriada. Não alterne se:

- Seu aplicativo usa extensões de diretório criadas por meio do AD Connect
- Seu aplicativo define valores de extensão de diretório que são usados em declarações de token por outros aplicativos
- Seu aplicativo define valores de extensão de diretório que são usados em regras de associação dinâmica 

>**OBSERVAÇÃO**: ainda não há suporte para o uso de propriedades de extensão de esquema do Microsoft Graph como declarações em um token usando declarações opcionais ou em uma regra de associação dinâmica.

Para alternar para o modelo de extensão de esquema do Microsoft Graph mais recente, você precisará:

- Defina novas definições de extensão de esquema usando o Microsoft Graph.
- Atualize o aplicativo para dar suporte às novas definições de extensão de esquema.
- Migre os dados das propriedades de extensão Azure AD esquema para as novas propriedades de extensão de esquema do Microsoft Graph.  Não há suporte para migração automática de dados.

## <a name="differential-queries"></a>Consultas diferenciais

Azure AD Graph e o Microsoft Graph permitem que você acompanhe as alterações usando consultas.  A abordagem de alto nível é semelhante entre as duas APIs, mas a sintaxe é diferente.

Azure AD Graph chama essas consultas diferenciais.  No Microsoft Graph, elas são consultas [delta](./delta-query-overview.md).

A tabela a seguir destaca as principais semelhanças e diferenças:

|Solicitação delta |Azure AD Graph. | Microsoft Graph |
|----|----|----|
| _Solicitação de dados inicial_ | Usa um parâmetro de consulta:<br>`GET /groups?deltaLink=` | Usa uma função: <br> `GET /groups/delta` |
| _Obter novas alterações_ | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| _Sincronizar a partir de agora_ |Usa um cabeçalho HTTP personalizado:<br> `ocp-aad-dq-include-only-delta-token: true` | Usa um parâmetro de consulta: <br> `GET /groups/delta?$deltaToken=latest` |
| _Controlar alterações para directoryObjects_ | Obtém alterações para vários recursos (usuário e grupo) na mesma operação:&nbsp;&nbsp;<br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | Usa consultas separadas com o Microsoft Graph, uma para cada recurso. |
| _Obter alterações de recursos e relações_ | Todas as solicitações retornam alterações de relação e recurso, se o recurso tiver relações. | `GET /groups/delta?$expand=members` |
| _Resposta indicando itens novos e alterados_ | <ul><li><p>Representa instâncias recém-criadas usando sua representação padrão.</p></li><li><p>As instâncias atualizadas são representadas por sua ID com *pelo menos* as propriedades que foram atualizadas. Outras propriedades podem ser incluídas.</p></li><li><p>As relações são representadas como o `directoryLinkChange` tipo.</p></li></ul>|<ul><li><p>Representa instâncias recém-criadas usando sua representação padrão.</p></li><li><p>As instâncias atualizadas são representadas por sua ID com *pelo menos* as propriedades que foram atualizadas. Outras propriedades podem ser incluídas.</p></li><li><p>As relações são representadas como anotações na representação de recurso padrão. Essas anotações usam o formato `propertyName@delta`, por exemplo `members@delta` , para as alterações de associação de um grupo.</p></li></ul> |
| _Resposta indicando itens excluídos_| Indica um item excluído com uma propriedade adicional *de aad.isDeleted* definida como true. | Indica um item excluído com a \@anotação removida. Ele também pode conter um código de motivo, que indica se o item foi excluído, mas pode ser restaurado ou excluído permanentemente. |

Se seu aplicativo já estiver armazenando dados de estado, considere usar a "sincronização a partir de agora" mostrada anteriormente para ajudar a gerenciar a transição para consultas delta.

## <a name="batching"></a>Envio em lote

Azure AD Graph usou um sistema chamado mensagens MIME de várias partes para gerenciar o envio em lote.  O Microsoft Graph usa [o envio em lote JSON](json-batching.md) para permitir até 20 solicitações em uma única operação em lote. O mecanismo de envio em lote JSON é significativamente mais simples de usar, especialmente junto com bibliotecas de análise JSON.  Ele também permite o sequenciamento de operações em lote.  No entanto, ele não é compatível com versões anteriores com a abordagem Azure AD envio em lote do Graph.

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre as diferenças de](migrate-azure-ad-graph-resource-differences.md) recursos entre o Azure AD Graph e o Microsoft Graph.
- Examine a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->