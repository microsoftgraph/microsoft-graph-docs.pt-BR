---
title: tipo de recurso oAuth2PermissionGrant
description: Representa as permissões delegadas (escopos de OAuth 2,0) que foram concedidas a um aplicativo, com frequência como resultado de um usuário ou processo de consentimento de administrador.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bd88f0e7f323b3408e7552148db032c53bd03e94
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290108"
---
# <a name="oauth2permissiongrant-resource-type"></a>tipo de recurso oAuth2PermissionGrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as permissões delegadas que foram concedidas à entidade de serviço de um aplicativo.

Conceder permissões delegadas podem ser criadas como resultado de um usuário que esteja consentindo a solicitação de um aplicativo para acessar uma API ou criado diretamente.

As permissões delegadas às vezes são chamadas de "escopos de OAuth 2,0" ou "escopos".

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Listar oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) collection | Recupere uma lista de subsídios de permissão delegada. |
| [Obter oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | Leia uma única concessão de permissão delegada.|
| [Criar oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | Criar uma concessão de permissão delegada. |
| [Atualizar oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | Nenhum | Atualize o objeto oAuth2PermissionGrant. |
| [Excluir oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Nenhum  | Excluir uma concessão de permissão delegada. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Identificador exclusivo para o **oAuth2PermissionGrant**. Somente leitura.|
| clientId | String | A **ID** da entidade de [serviço](serviceprincipal.md) do cliente para o aplicativo que é autorizado a atuar em nome de um usuário conectado ao acessar uma API. Obrigatório. Suporta `$filter` ( `eq` somente). |
| consentType | String | Indica se a autorização é concedida para que o aplicativo cliente represente todos os usuários ou apenas um usuário específico. A *entidade de segurança* indica autorização para representar todos os usuários. *Principal* indica autorização para representar um usuário específico. O consentimento em nome de todos os usuários pode ser concedido por um administrador. Os usuários que não são administradores podem ser autorizados a consentir em nome de alguns casos, para algumas permissões delegadas. Obrigatório. Suporta `$filter` ( `eq` somente). |
| principalId | String | A **ID** do [usuário](user.md) em nome do qual o cliente está autorizado a acessar o recurso, quando **resenttype** é o *principal*. Se **consenttype** for *servicePrincipalName* , esse valor será NULL. Obrigatório quando **resenttype** é *principal*. |
| resourceId | Cadeia de caracteres | A **ID** da entidade de [serviço](serviceprincipal.md) de recurso para a qual o acesso é autorizado. Isso identifica a API que o cliente está autorizado a tentar chamar em nome de um usuário conectado. |
| escopo | String | Uma lista separada por espaços dos valores de declaração para permissões delegadas que devem ser incluídas em tokens de acesso para o aplicativo de recurso (a API). Por exemplo, `openid User.Read GroupMember.Read.All`. Cada valor de declaração deve corresponder ao campo de **valor** de uma das permissões delegadas definidas pela API, listadas na propriedade **publishedPermissionScopes** da entidade de [serviço](serviceprincipal.md)de recurso. |
| startTime | DateTimeOffset | No momento, o valor de hora de início é ignorado, mas um valor é necessário ao criar **oAuth2PermissionGrant**. Obrigatório. |
| expiryTime | DateTimeOffset | No momento, o valor de hora de término é ignorado, mas um valor é necessário ao criar **oAuth2PermissionGrant**. Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/oauth2permissiongrant-delta.md).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) collection | Recupere uma lista de objetos **oauth2PermissionGrant** . |
|[Obter oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Leia as propriedades e os relacionamentos de um objeto **oAuth2PermissionGrant** .|
|[Atualizar oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Atualize um objeto **oAuth2PermissionGrant** . |
|[Excluir oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Nenhum |Excluir um objeto **oAuth2PermissionGrant** . |
|[Obter delta](../api/oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](oauth2permissiongrant.md)|Obter objetos **oauth2permissiongrant** recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|clientId|String| A ID da entidade de serviço que recebe o consentimento para representar o usuário ao acessar o recurso (representado pela Propriedade ResourceId). |
|consentType|String| Indica se o consentimento foi fornecido pelo administrador (em nome da organização) ou por um indivíduo. Os valores possíveis são *Userdirigetes* ou *entidade de segurança*. |
|expiryTime|DateTimeOffset| No momento, o valor de tempo de expiração é ignorado. |
|id|String| Identificador exclusivo. Somente leitura.|
|principalId|String| Se consenttype for *servicePrincipalName* , esse valor será nulo e o consentimento se aplicará a todos os usuários da organização. Se consenttype for *principal*, essa propriedade especificará a ID do usuário que receberá o consentimento e se aplicará somente para esse usuário. |
|resourceId|Cadeia de caracteres| Especifica a ID da entidade de serviço de recurso para a qual o acesso foi concedido. |
|escopo|String| Especifica o valor da declaração do [escopo](/graph/permissions-reference) que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0. Por exemplo, *User. Read* |
|startTime|DateTimeOffset| No momento, o valor de hora de início é ignorado. |

## <a name="relationships"></a>Relações
Nenhum

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
  "scope": "string",
  "startTime": "String (timestamp)",
  "expiryTime": "String (timestamp)"
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
