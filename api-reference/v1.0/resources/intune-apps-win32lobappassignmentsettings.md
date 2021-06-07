---
title: Tipo de recurso win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel LOB win32 a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d76e189d684999e3922b625def26d4d0cfcb6a3e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752207"
---
# <a name="win32lobappassignmentsettings-resource-type"></a>Tipo de recurso win32LobAppAssignmentSettings

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um aplicativo móvel LOB win32 a um grupo.


Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|notificações|[win32LobAppNotification](../resources/intune-apps-win32lobappnotification.md)|O status de notificação para essa atribuição de aplicativo. Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.|
|restartSettings|[win32LobAppRestartSettings](../resources/intune-apps-win32lobapprestartsettings.md)|As configurações de reinicialização a ser aplicadas a essa atribuição de aplicativo.|
|installTimeSettings|[mobileAppInstallTimeSettings](../resources/intune-apps-mobileappinstalltimesettings.md)|As configurações de tempo de instalação a ser aplicadas a essa atribuição de aplicativo.|
|deliveryOptimizationPriority|[win32LobAppDeliveryOptimizationPriority](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|A prioridade de otimização de entrega para essa atribuição de aplicativo. Essa configuração não é suportada em ambientes de Nuvem Nacional. Os valores possíveis são: `notConfigured`, `foreground`.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String",
  "restartSettings": {
    "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
    "gracePeriodInMinutes": 1024,
    "countdownDisplayBeforeRestartInMinutes": 1024,
    "restartNotificationSnoozeDurationInMinutes": 1024
  },
  "installTimeSettings": {
    "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
    "useLocalTime": true,
    "startDateTime": "String (timestamp)",
    "deadlineDateTime": "String (timestamp)"
  },
  "deliveryOptimizationPriority": "String"
}
```




