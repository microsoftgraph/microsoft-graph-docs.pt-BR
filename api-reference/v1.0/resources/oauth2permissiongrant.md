---
title: Tipo de recurso oAuth2PermissionGrant
description: Representa as permissões delegadas (escopos do OAuth 2.0) que foram concedidas a um aplicativo, geralmente como resultado do processo de consentimento do usuário ou administrador.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 300c44691aab3cc8f09bf621dd39bd89825dee2a
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118449"
---
# <a name="oauth2permissiongrant-resource-type"></a>Tipo de recurso oAuth2PermissionGrant

Namespace: microsoft.graph

Representa as permissões delegadas que foram concedidas à entidade de serviço de um aplicativo.

As concessões de permissões delegadas podem ser criadas como resultado de um usuário consentir a solicitação de um aplicativo para acessar uma API ou ser criado diretamente.

As permissões delegadas às vezes são chamadas de "escopos do OAuth 2.0" ou "escopos".

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Listar oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) collection | Recupere uma lista de concessões de permissão delegadas. |
| [Obter oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | Ler uma única concessão de permissão delegada.|
| [Criar oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | Crie uma concessão de permissão delegada. |
| [Atualizar oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | Nenhuma | Atualize o objeto oAuth2PermissionGrant. |
| [Excluir oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Nenhuma  | Exclua uma concessão de permissão delegada. |
|[Obter delta](../api/oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](oauth2permissiongrant.md)|Obtenha objetos **oauth2permissiongrant** recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | Cadeia de caracteres | Identificador exclusivo para **o oAuth2PermissionGrant**. Somente leitura.|
| clientId | Cadeia de caracteres | A **ID** da entidade de [](serviceprincipal.md) serviço do cliente para o aplicativo que está autorizado a agir em nome de um usuário conectado ao acessar uma API. Obrigatório. Suporte para `$filter` (`eq` somente). |
| consentType | Cadeia de caracteres | Indica se a autorização é concedida para que o aplicativo cliente represente todos os usuários ou apenas um usuário específico. *AllPrincipals* indica autorização para representar todos os usuários. *A entidade* de segurança indica autorização para representar um usuário específico. O consentimento em nome de todos os usuários pode ser concedido por um administrador. Usuários não administradores podem estar autorizados a consentir em nome de si mesmos em alguns casos, para algumas permissões delegadas. Obrigatório. Suporte para `$filter` (`eq` somente). |
| principalId | Cadeia de caracteres | A **ID** do usuário [em](user.md) nome do qual o cliente está autorizado a acessar o recurso, quando **consentType** é *Principal*. Se **consentType** for *AllPrincipals* , esse valor será nulo. Obrigatório quando **consentType** é *Principal*. Suporte para `$filter` (`eq` somente).|
| resourceId | Cadeia de caracteres | A **ID da** entidade de [serviço de recurso](serviceprincipal.md) à qual o acesso está autorizado. Isso identifica a API que o cliente está autorizado a tentar chamar em nome de um usuário conectado. Suporte para `$filter` (`eq` somente). |
| escopo | String | Uma lista separada por espaço dos valores de declaração para permissões delegadas que devem ser incluídos em tokens de acesso para o aplicativo de recurso (a API). Por exemplo, `openid User.Read GroupMember.Read.All`. Cada valor de declaração deve corresponder  ao campo de valor de uma das permissões delegadas definidas pela API, listadas na propriedade **oauth2PermissionScopes** da entidade de serviço [de recurso](serviceprincipal.md). |

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

