---
title: tipo de recurso de privilegedRoleSettings
description: Representa as configurações para uma função privilegiada.
localization_priority: Normal
ms.openlocfilehash: 673327e3c83a4111eb469ca48550836433dbdf0a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577148"
---
# <a name="privilegedrolesettings-resource-type"></a>tipo de recurso de privilegedRoleSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações para uma função privilegiada.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.|
|[Atualizar privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Atualize o objeto privilegedRoleSettings.|
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|elevationDuration| Cadeia de caracteres (timestamp) |A duração quando a função for ativada.|
|id| cadeia de caracteres (identificador)| O identificador exclusivo para as configurações de função. Somente leitura.|
|isMfaOnElevationConfigurable|booliano|**true** se mfaOnElevation é configurável. **false** se mfaOnElevation não é configurável.|
|lastGlobalAdmin|booliano|Interno usado apenas.|
|maxElavationDuration| cadeia de caracteres (identificador)| |Duração máxima para a função ativada.|
|mfaOnElevation|booliano|**true** se MFA é necessária para ativar a função. **false** se MFA não é necessário para ativar a função.|
|minElevationDuration|cadeia de caracteres (identificador)||Duração mínima para a função ativada.|
|notificationToUserOnElevation|booliano|**True** se enviar notificação ao usuário final quando a função é ativada. **False** se não enviar notificação quando a função é ativada.|
|ticketingInfoOnElevation|booliano|**true** se as informações de tickets são necessária quando ativar a função. **false** se as informações de tickets não são necessária quando ativar a função.|
|approvalOnElevation|booliano|**true** se a aprovação é necessária quando ativar a função. **false** se a aprovação não é necessária quando ativar a função.|
|approverIds| String collection |Lista de ids de aprovação, se a aprovação é necessária para a ativação.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": [ "String (identifier)" ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
