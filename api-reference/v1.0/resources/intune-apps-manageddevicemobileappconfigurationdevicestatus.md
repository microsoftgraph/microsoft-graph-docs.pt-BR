---
title: tipo de recurso de managedDeviceMobileAppConfigurationDeviceStatus
description: Contém propriedades, as propriedades herdadas e ações para um status de configuração de aplicativos móveis MDM para um dispositivo.
localization_priority: Normal
ms.openlocfilehash: 9698c249d8075a7567c3f54defa3d20a475174ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841437"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a>tipo de recurso de managedDeviceMobileAppConfigurationDeviceStatus

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades, as propriedades herdadas e ações para um status de configuração de aplicativos móveis MDM para um dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista managedDeviceMobileAppConfigurationDeviceStatuses](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Lista as propriedades e os relacionamentos dos objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .|
|[Obter managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Leia as propriedades e os relacionamentos do objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .|
|[Criar managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Crie um novo objeto de [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .|
|[Excluir managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|Nenhum|Exclui um [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).|
|[Atualizar managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Atualize as propriedades de um objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
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
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



