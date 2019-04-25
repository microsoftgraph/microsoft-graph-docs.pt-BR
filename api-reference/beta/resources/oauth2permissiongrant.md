---
title: tipo de recurso oAuth2PermissionGrant
description: Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581524"
---
# <a name="oauth2permissiongrant-resource-type"></a>tipo de recurso oAuth2PermissionGrant

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
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
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|clientId|String| A ID da entidade de serviço que recebe o consentimento para representar o usuário ao acessar o recurso (representado pela propriedade reSourceid). |
|consentType|String| Indica se o consentimento foi fornecido pelo administrador (em nome da organização) ou por um indivíduo. Os valores possíveis são ** userdirigetes ou *entidade de segurança*. |
|expiryTime|DateTimeOffset| No momento, o valor de tempo de expiração é ignorado. |
|id|String| Identificador exclusivo. Somente leitura.|
|principalId|String| Se consenttype for *servicePrincipalName* , esse valor será nulo e o consentimento se aplicará a todos os usuários da organização. Se consenttype for *principal*, essa propriedade especificará a ID do usuário que receberá o consentimento e se aplicará somente para esse usuário. |
|resourceId|String| Especifica a ID da entidade de serviço de recurso para a qual o acesso foi concedido. |
|escopo|String| Especifica o valor da declaração do [escopo](/graph/permissions-reference) que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0. Por exemplo, *User. Read* |
|startTime|DateTimeOffset| No momento, o valor de hora de início é ignorado. |

## <a name="relationships"></a>Relações
Nenhuma


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Leia as propriedades e os relacionamentos do objeto oAuth2PermissionGrant.|
|[Listar oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) collection | Recupere uma lista de objetos oauth2PermissionGrant. |
|[Atualizar oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Atualize o objeto oAuth2PermissionGrant. |
|[Excluir oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Nenhum |Exclua o objeto oAuth2PermissionGrant. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permissiongrant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
