---
title: tipo de recurso iosVppAppRevokeLicensesActionResult
description: Define resultados para ações em aplicativos VPP do iOS, contendo propriedades herdadas de ActionResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f101784808e20566deb59b2e3f61cb886371c17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005461"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a>tipo de recurso iosVppAppRevokeLicensesActionResult

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Define resultados para ações em aplicativos VPP do iOS, contendo propriedades herdadas de ActionResult.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userId|Cadeia de caracteres|UserId associado à ação.|
|managedDeviceId|String|DeviceID associado à ação.|
|totalLicensesCount|Int32|Uma contagem do número de licenças para as quais houve uma tentativa de revogação.|
|failedLicensesCount|Int32|Uma contagem do número de licenças para as quais houve falha na revogação.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|O motivo da falha na ação de revogação de licenças. Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|
|actionName|Cadeia de caracteres|Nome da ação|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Estado da ação. Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Hora em que a ação foi iniciada|
|lastUpdatedDateTime|DateTimeOffset|Hora da última atualização do estado da ação|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





