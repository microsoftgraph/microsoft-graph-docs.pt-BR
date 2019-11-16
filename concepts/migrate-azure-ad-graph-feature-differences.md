---
title: Diferenças de recursos entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças de recursos entre a API do Azure Active Directory (Azure AD) e a API do Microsoft Graph para ajudá-lo a migrar aplicativos de forma rápida e fácil.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1e99c5e0c6b2df9e30787481c36a32dcd65485d8
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38656533"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de recursos entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: revisar as diferenças de API* do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Muitos recursos do Microsoft Graph funcionam de forma semelhante aos seus colegas do Azure AD Graph. No entanto, alguns foram alterados e/ou aprimorados. Aqui, você aprenderá como adaptar seus aplicativos para aproveitar essas diferenças.  Frequentemente, as alterações são secundárias, mas vale a pena.

Este artigo explora como o Microsoft Graph trata:

- Extensões de esquema de diretório
- Consultas diferenciais
- Envio em lote

## <a name="directory-schema-extensions"></a>Extensões de esquema de diretório

Se o aplicativo usar extensões de esquema de diretório do Azure AD Graph, você poderá continuar usando as mesmas APIs básicas (com as URLs de solicitação do Microsoft Graph) para:

- Gerenciar definições de propriedade de extensão usando a propriedade **extensionproperties** no recurso [Application] [/Graph/API/Resources/Application? View = Graph-REST-v 1.0).
- Ler valores de extensão usando GET e`$select`
- Pesquisar valores de extensão usando GET e`$filter`
- Atualizar valores de extensão usando PATCH
- Remover valores de extensão usando PATCH (definido como **nulo**)

O Microsoft Graph fornece uma experiência de desenvolvedor aprimorada de extensões de esquema, que hoje não é compatível com versões anteriores com extensões de esquema de diretório do Azure AD Graph. Para saber mais, veja [extensões de esquema em adicionar dados personalizados](/graph/extensibility-overview#schema-extensions).

### <a name="recommended-migration-approach"></a>Abordagem de migração recomendada

Se seu aplicativo do Azure AD Graph usa extensões de esquema de diretório, faça uma abordagem incremental para migrar o aplicativo para o Microsoft Graph.

Primeiro, alterne seu aplicativo para usar chamadas da API do Microsoft Graph, mas deixe que o aplicativo continue a aproveitar as extensões de esquema de diretório do Azure AD Graph.

Em seguida, você pode alternar para usar extensões de esquema do Microsoft Graph. Em alguns casos, a alternância não será apropriada. Não alternar se:

- Seu aplicativo usa extensões de esquema de diretório criadas por meio do AD Connect ou
- Seu aplicativo depende dos valores de extensão do esquema de diretório nas declarações de token.

>**Observação**: o uso de propriedades de extensão de esquema do Microsoft Graph como declarações em um token que usa declarações opcionais ou em uma regra de associação dinâmica também não tem suporte.

Para alternar para o modelo de extensão de esquema do Microsoft Graph mais recente, você precisará:

- Definir novas definições de extensão de esquema usando o Microsoft Graph.
- Atualize o aplicativo para dar suporte às novas definições de extensão de esquema.
- Migre os dados das propriedades de extensão de esquema do Azure AD para as novas propriedades de extensão de esquema do Microsoft Graph.  Não há suporte para a migração automática de dados.

## <a name="differential-queries"></a>Consultas diferenciais

O Azure AD Graph e o Microsoft Graph permitem que você controle alterações usando consultas.  A abordagem de alto nível é semelhante entre as duas APIs, mas a sintaxe é diferente.  

O Azure AD Graph chama essas consultas diferenciais.  No Microsoft Graph, eles são [consultas Delta](/graph/delta-query-overview).

A tabela a seguir destaca as principais semelhanças e diferenças:

||Azure AD Graph. | Microsoft Graph |
|----|----|----|
| _Solicitação de dados inicial_ | Usa um parâmetro de consulta:<br>`GET /groups?deltaLink=` | O usa uma função: <br> `GET /groups/delta` |
| _Obter novas alterações_ | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| _Sincronizar a partir de agora_ |Usa um cabeçalho HTTP personalizado:<br> `ocp-aad-dq-include-only-delta-token: true` | Usa um parâmetro de consulta: <br> `GET /groups/delta?$deltaToken=latest` |
| _Controlar alterações para o directoryObjects_ | Obtém alterações para vários recursos (usuário e grupo) na mesma operação:&nbsp;&nbsp;<br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | Usa consultas separadas com o Microsoft Graph, uma para cada recurso. |
| _Obter alterações de recursos e relações_ | Todas as solicitações retornam as alterações de recurso e relação, se o recurso tiver relações. | `GET /groups/delta?$expand=members` |
| _Resposta que indica itens novos e alterados_ | <ul><li><p>Representa instâncias recém-criadas usando sua representação padrão.</p></li><li><p>As instâncias atualizadas são representadas por sua ID com *pelo menos* as propriedades que foram atualizadas. Outras propriedades podem ser incluídas.</p></li><li><p>As relações são representadas `directoryLinkChange` como o tipo.</p></li></ul>|<ul><li><p>Representa instâncias recém-criadas usando sua representação padrão.</p></li><li><p>As instâncias atualizadas são representadas por sua ID com *pelo menos* as propriedades que foram atualizadas. Outras propriedades podem ser incluídas.</p></li><li><p>As relações são representadas como anotações na representação de recursos padrão. Essas anotações usam o formato `propertyName@delta`, por exemplo `members@delta` , para as alterações de associação de um grupo.</p></li></ul> |
| _Resposta indicando itens excluídos_| Indica um item excluído com uma propriedade adicional de *AAD. IsDeleted* definida como true. | Indica um item excluído com a \@anotação removida. Ele também pode conter um código de motivo, que indica se o item foi excluído, mas pode ser restaurado ou excluído permanentemente. |

Se seu aplicativo já estiver armazenando dados de estado, considere o uso de "sincronizar a partir de agora" mostrado anteriormente para ajudar a gerenciar a transição para consultas Delta.

## <a name="batching"></a>Envio em lote

O Azure AD Graph usava um sistema chamado mensagens MIME de várias partes para gerenciar o envio em lote.  O Microsoft Graph usa o [processamento em lotes JSON](json-batching.md) para permitir até 20 solicitações em uma única operação em lote. O mecanismo de lote JSON é muito mais simples de usar, especialmente em conjunto com as bibliotecas de análise JSON.  Também permite operações em lote de sequenciamento.  No entanto, não é compatível com versões anteriores da abordagem de lotes do Azure AD Graph.

## <a name="next-steps"></a>Próximos passos

- Saiba mais sobre as [diferenças de recursos](migrate-azure-ad-graph-resource-differences.md) entre o Azure ad Graph e o Microsoft Graph.
- Explore [Adicionar dados personalizados](/graph/extensibility-overview) para obter informações sobre as extensões abertas e de esquema.
- Explore as [consultas Delta](/graph/delta-query-overview) para saber mais sobre a versão do Microsoft Graph da consulta diferencial.
- Explore o [processamento em lotes JSON](json-batching.md) para entender como o processamento em lotes funciona no Microsoft Graph.
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->
