---
title: Tipo de recurso iosUpdateDeviceStatus
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: ee7366c83cbe8a65c128944cc17abfc9dd2cf0df
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309244"
---
# <a name="iosupdatedevicestatus-resource-type"></a>Tipo de recurso iosUpdateDeviceStatus

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosUpdateDeviceStatuses](../api/intune-deviceconfig-iosupdatedevicestatus-list.md)|Conjunto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Listar propriedades e relações de objetos de [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|
|[Obter iosUpdateDeviceStatus](../api/intune-deviceconfig-iosupdatedevicestatus-get.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Ler propriedades e relações de objetos de [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|
|[Criar iosUpdateDeviceStatus](../api/intune-deviceconfig-iosupdatedevicestatus-create.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Criar um novo objeto de [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|
|[Excluir iosUpdateDeviceStatus](../api/intune-deviceconfig-iosupdatedevicestatus-delete.md)|Nenhum|Excluir [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|
|[Atualizar iosUpdateDeviceStatus](../api/intune-deviceconfig-iosupdatedevicestatus-update.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Atualizar as propriedades de um objeto de [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|installStatus|[iosUpdatesInstallStatus](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|O status de instalação do relatório de políticas. Os valores possíveis são: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.|
|osVersion|Cadeia de caracteres|A versão do dispositivo que está sendo relatado.|
|deviceId|Cadeia de caracteres|A ID do dispositivo que está sendo relatado.|
|userId|Cadeia de caracteres|A ID do usuário que está sendo relatado.|
|deviceDisplayName|Cadeia de caracteres|Nome do dispositivo de DevicePolicyStatus.|
|userName|Cadeia de caracteres|O nome de usuário que está sendo relatado|
|deviceModel|Cadeia de caracteres|O modelo do dispositivo que está sendo relatado|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|DateTime em que o período de cortesia de conformidade do dispositivo termina|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Status de conformidade do relatório de políticas. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Data e hora da última modificação do relatório de políticas.|
|userPrincipalName|Cadeia de caracteres|UserPrincipalName.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "String (identifier)",
  "installStatus": "String",
  "osVersion": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



