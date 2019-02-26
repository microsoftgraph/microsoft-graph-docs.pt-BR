---
title: tipo de recurso macOsVppAppRevokeLicensesActionResult
description: Define os resultados de ações em aplicativos de conteúdo do MacOS, que contém as propriedades herdadas de ActionResult.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cf8390dc2c1541525e288b81defd073144f4132
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166504"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a>tipo de recurso macOsVppAppRevokeLicensesActionResult

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Define os resultados de ações em aplicativos de conteúdo do MacOS, que contém as propriedades herdadas de ActionResult.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userId|String|UserId associado à ação.|
|managedDeviceId|String|DeViceid associado à ação.|
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
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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




