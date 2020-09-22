---
title: tipo de recurso oAuth2PermissionGrant
description: Representa as permissões delegadas (escopos de OAuth 2,0) que foram concedidas a um aplicativo, com frequência como resultado de um usuário ou processo de consentimento de administrador.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 557bd9973a3a04ffedb2104a480823de21c95499
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041194"
---
# <a name="oauth2permissiongrant-resource-type"></a>tipo de recurso oAuth2PermissionGrant

Namespace: microsoft.graph

Representa as permissões delegadas que foram concedidas à entidade de serviço de um aplicativo.

Conceder permissões delegadas podem ser criadas como resultado de um usuário que esteja consentindo a solicitação de um aplicativo para acessar uma API ou criado diretamente.

As permissões delegadas às vezes são chamadas de "escopos de OAuth 2,0" ou "escopos".

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Listar oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) collection | Recupere uma lista de subsídios de permissão delegada. |
| [Obter oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | Leia uma única concessão de permissão delegada.|
| [Criar oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | Criar uma concessão de permissão delegada. |
| [Atualizar oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | Nenhum | Atualize o objeto oAuth2PermissionGrant. |
| [Excluir oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Nenhum  | Excluir uma concessão de permissão delegada. |
|[Obter delta](../api/oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](oauth2permissiongrant.md)|Obter objetos **oauth2permissiongrant** recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Identificador exclusivo para o **oAuth2PermissionGrant**. Somente leitura.|
| clientId | Cadeia de caracteres | A **ID** da entidade de [serviço](serviceprincipal.md) do cliente para o aplicativo que é autorizado a atuar em nome de um usuário conectado ao acessar uma API. Obrigatório. Suporta `$filter` ( `eq` somente). |
| consentType | String | Indica se a autorização é concedida para que o aplicativo cliente represente todos os usuários ou apenas um usuário específico. A *entidade de segurança* indica autorização para representar todos os usuários. *Principal* indica autorização para representar um usuário específico. O consentimento em nome de todos os usuários pode ser concedido por um administrador. Os usuários que não são administradores podem ser autorizados a consentir em nome de alguns casos, para algumas permissões delegadas. Obrigatório. Suporta `$filter` ( `eq` somente). |
| principalId | String | A **ID** do [usuário](user.md) em nome do qual o cliente está autorizado a acessar o recurso, quando **resenttype** é o *principal*. Se **consenttype** for *servicePrincipalName* , esse valor será NULL. Obrigatório quando **resenttype** é *principal*. |
| resourceId | Cadeia de caracteres | A **ID** da entidade de [serviço](serviceprincipal.md) de recurso para a qual o acesso é autorizado. Isso identifica a API que o cliente está autorizado a tentar chamar em nome de um usuário conectado. |
| escopo | String | Uma lista separada por espaços dos valores de declaração para permissões delegadas que devem ser incluídas em tokens de acesso para o aplicativo de recurso (a API). Por exemplo, `openid User.Read GroupMember.Read.All`. Cada valor de declaração deve corresponder ao campo de **valor** de uma das permissões delegadas definidas pela API, listadas na propriedade **publishedPermissionScopes** da entidade de [serviço](serviceprincipal.md)de recurso. |

## <a name="relationships"></a>Relações

Nenhum

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/oauth2permissiongrant-delta.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

