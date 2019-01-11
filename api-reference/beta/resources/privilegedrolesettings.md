---
title: tipo de recurso de privilegedRoleSettings
description: Representa as configurações para uma função privilegiada.
localization_priority: Normal
ms.openlocfilehash: 971c48ce3ecdd2a219a111f3a11884377e20430c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842739"
---
# <a name="privilegedrolesettings-resource-type"></a>tipo de recurso de privilegedRoleSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa as configurações para uma função privilegiada.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.|
|[Atualizar privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Atualize o objeto privilegedRoleSettings.|
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|elevationDuration|duration|A duração quando a função for ativada.|
|id|string| O identificador exclusivo para as configurações de função. Somente leitura.|
|isMfaOnElevationConfigurable|booliano|**true** se mfaOnElevation é configurável. **false** se mfaOnElevation não é configurável.|
|lastGlobalAdmin|booliano|Interno usado apenas.|
|maxElavationDuration|duration|Duração máxima para a função ativada.|
|mfaOnElevation|booliano|**true** se MFA é necessária para ativar a função. **false** se MFA não é necessário para ativar a função.|
|minElevationDuration|duration|Duração mínima para a função ativada.|
|notificationToUserOnElevation|booliano|**True** se enviar notificação ao usuário final quando a função é ativada. **False** se não enviar notificação quando a função é ativada.|
|ticketingInfoOnElevation|booliano|**true** se as informações de tickets são necessária quando ativar a função. **false** se as informações de tickets não são necessária quando ativar a função.|
|approvalOnElevation|booliano|**true** se a aprovação é necessária quando ativar a função. **false** se a aprovação não é necessária quando ativar a função.|
|approverIds|array|Lista de ids de aprovação, se a aprovação é necessária para a ativação.|

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
  "approverIds": []
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
