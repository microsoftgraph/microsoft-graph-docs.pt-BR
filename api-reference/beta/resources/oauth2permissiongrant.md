---
title: Tipo de recurso oAuth2PermissionGrant
description: Representa as permissões delegadas (escopos OAuth 2.0) que foram concedidas a um aplicativo, geralmente como resultado do processo de consentimento do usuário ou administrador.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 944a96858bea7a1e46ea1f59ef6b67092e4b06a6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442927"
---
# <a name="oauth2permissiongrant-resource-type"></a>Tipo de recurso oAuth2PermissionGrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as permissões delegadas que foram concedidas à entidade de serviço de um aplicativo.

As concessões de permissões delegadas podem ser criadas como resultado de um usuário consentir a solicitação de um aplicativo para acessar uma API ou criado diretamente.

As permissões delegadas às vezes são conhecidas como "escopos OAuth 2.0" ou "escopos".

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Listar oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) collection | Recupere uma lista de concessões de permissão delegadas. |
| [Obter oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | Leia uma única concessão de permissão delegada.|
| [Criar oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | Crie uma concessão de permissão delegada. |
| [Atualizar oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | Nenhum(a) | Atualizar o objeto oAuth2PermissionGrant. |
| [Excluir oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Nenhum(a)  | Exclua uma concessão de permissão delegada. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Identificador exclusivo do **oAuth2PermissionGrant**. Somente leitura.|
| clientId | Cadeia de caracteres | A **id** da [](serviceprincipal.md) entidade de serviço do cliente para o aplicativo que está autorizado a agir em nome de um usuário interno ao acessar uma API. Obrigatório. Suporte para `$filter` (`eq` somente). |
| consentType | String | Indica se a autorização é concedida para que o aplicativo cliente represente todos os usuários ou apenas um usuário específico. *AllPrincipals* indica autorização para representar todos os usuários. *A* entidade indica autorização para representar um usuário específico. O consentimento em nome de todos os usuários pode ser concedido por um administrador. Os usuários que não são administradores podem ser autorizados a consentir em nome de si mesmos em alguns casos, para algumas permissões delegadas. Obrigatório. Suporte para `$filter` (`eq` somente). |
| principalId | String | A **id** do [usuário em](user.md) nome do qual o cliente está autorizado a acessar o recurso, quando **consentType** for *Principal*. Se **consentType** for *AllPrincipals,* esse valor será nulo. Obrigatório quando **consentType** for *Principal*. |
| resourceId | Cadeia de caracteres | A **id da** entidade de [serviço de recursos](serviceprincipal.md) à qual o acesso está autorizado. Isso identifica a API que o cliente está autorizado a tentar chamar em nome de um usuário in-locar. |
| escopo | String | Uma lista separada por espaço dos valores de declaração para permissões delegadas que devem ser incluídos em tokens de acesso para o aplicativo de recurso (a API). Por exemplo, `openid User.Read GroupMember.Read.All`. Cada valor de  declaração deve corresponder ao campo de valor de uma das permissões delegadas definidas pela API, listadas na propriedade **publishedPermissionScopes** da entidade de [serviço de recursos](serviceprincipal.md). |
| startTime | DateTimeOffset | Atualmente, o valor da hora de início é ignorado, mas um valor é necessário ao criar **um oAuth2PermissionGrant**. Obrigatório. |
| expiryTime | DateTimeOffset | Atualmente, o valor de hora de término é ignorado, mas um valor é necessário ao criar **um oAuth2PermissionGrant**. Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/oauth2permissiongrant-delta.md).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) collection | Recupere uma lista de **objetos oauth2PermissionGrant.** |
|[Obter oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Leia as propriedades e as relações de um **objeto oAuth2PermissionGrant.**|
|[Atualizar oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Atualize **um objeto oAuth2PermissionGrant.** |
|[Excluir oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Nenhum(a) |**Exclua um objeto oAuth2PermissionGrant.** |
|[Obter delta](../api/oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](oauth2permissiongrant.md)|Obter objetos **oauth2permissiongrant** recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres| A id da entidade de serviço concedeu consentimento para representar o usuário ao acessar o recurso (representado pela propriedade resourceId). |
|consentType|String| Indica se o consentimento foi fornecido pelo administrador (em nome da organização) ou por um indivíduo. Os valores possíveis *são AllPrincipals* ou *Principal*. |
|expiryTime|DateTimeOffset| Atualmente, o valor de tempo de expiração é ignorado. |
|id|String| Identificador exclusivo. Somente leitura.|
|principalId|String| Se consentType for *AllPrincipals,* esse valor será nulo e o consentimento se aplicará a todos os usuários da organização. Se consentType for *Principal*, essa propriedade especificará a id do usuário que concedeu consentimento e se aplica somente a esse usuário. |
|resourceId|Cadeia de caracteres| Especifica a id da entidade de serviço de recursos à qual o acesso foi concedido. |
|escopo|String| Especifica o valor da declaração [de escopo](/graph/permissions-reference) que o aplicativo de recurso deve esperar no token de acesso OAuth 2.0. Por exemplo, *User.Read* |
|startTime|DateTimeOffset| Atualmente, o valor da hora de início é ignorado. |

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


