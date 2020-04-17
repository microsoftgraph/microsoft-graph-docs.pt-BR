---
title: tipo de recurso oAuth2PermissionGrant
description: Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f00d9aa79e6a18e5dddf6881e251b3cbf00172e6
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543412"
---
# <a name="oauth2permissiongrant-resource-type"></a>tipo de recurso oAuth2PermissionGrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.

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
|id|String| Identificador exclusivo. Apenas leitura.|
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
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
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
