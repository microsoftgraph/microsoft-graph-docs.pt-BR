---
title: tipo de recurso privilegedRoleSettings
description: Representa as configurações de uma função privilegiada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c072f75095267910d128396c3848b2decca4728c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521492"
---
# <a name="privilegedrolesettings-resource-type"></a>tipo de recurso privilegedRoleSettings

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de uma função privilegiada.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.|
|[Atualizar privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Atualize o objeto privilegedRoleSettings.|
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|elevationDuration|duration|A duração quando a função é ativada.|
|id|string| O identificador exclusivo das configurações de função. Somente leitura.|
|isMfaOnElevationConfigurable|booliano|**true** se mfaOnElevation é configurável. **false** se mfaOnElevation não é configurável.|
|lastGlobalAdmin|booliano|Somente para uso interno.|
|maxElavationDuration|duration|Duração máxima da função ativada.|
|mfaOnElevation|booliano|**true** se a MFA é necessária para ativar a função. **false** se a MFA não é necessária para ativar a função.|
|minElevationDuration|duration|Duração mínima para a função ativada.|
|notificationToUserOnElevation|booliano|**true** se enviar notificação para o usuário final quando a função é ativada. **false** se não enviar notificações quando a função for ativada.|
|ticketingInfoOnElevation|booliano|**true** se as informações de tíquete são necessárias ao ativar a função. **false** se as informações de tíquete não são necessárias ao ativar a função.|
|approvalOnElevation|booliano|**true** se a aprovação é necessária ao ativar a função. **false** se a aprovação não é necessária ao ativar a função.|
|approverIds| coleção de cadeias de caracteres |Lista de IDs de aprovação, se a aprovação for necessária para ativação.|

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
  "approverIds": ["string"]
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
  "suppressions": []
}
-->
