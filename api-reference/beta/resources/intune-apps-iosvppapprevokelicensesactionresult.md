---
title: tipo de recurso de iosVppAppRevokeLicensesActionResult
description: Define os resultados para ações em iOS Vpp Apps, contém as propriedades herdadas para ActionResult.
localization_priority: Normal
ms.openlocfilehash: 8ed57465e263245cfc18ca22899c2142d949855d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842081"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a>tipo de recurso de iosVppAppRevokeLicensesActionResult

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Define os resultados para ações em iOS Vpp Apps, contém as propriedades herdadas para ActionResult.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userId|Cadeia de caracteres|ID de usuário associado à ação.|
|managedDeviceId|Cadeia de caracteres|DeviceId associado à ação.|
|totalLicensesCount|Int32|Uma contagem do número de licenças para o qual revoke foi tentada.|
|failedLicensesCount|Int32|Uma contagem do número de licenças para o qual revoke falhou.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|O motivo da falha de ação de licenças revoke. Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|
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





