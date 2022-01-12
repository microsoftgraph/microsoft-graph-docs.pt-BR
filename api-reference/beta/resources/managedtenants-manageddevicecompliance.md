---
title: Tipo de recurso managedDeviceCompliance
description: Representa o estado de conformidade do dispositivo para cada dispositivo gerenciado pertencente a um determinado locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: ce9f8ea1ed4e2a083daa053d17714569b4b2abfe
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61811161"
---
# <a name="manageddevicecompliance-resource-type"></a>Tipo de recurso managedDeviceCompliance

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado de conformidade do dispositivo para cada dispositivo gerenciado pertencente a um determinado locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceCompliances](../api/managedtenants-managedtenant-list-manageddevicecompliances.md)|[coleção microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md)|Obter uma lista dos [objetos managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) e suas propriedades.|
|[Obter managedDeviceCompliance](../api/managedtenants-manageddevicecompliance-get.md)|[microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md)|Leia as propriedades e as relações de um [objeto managedDeviceCompliance.](../resources/managedtenants-manageddevicecompliance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|complianceStatus|String|Estado de conformidade do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`. Opcional. Somente leitura.|
|deviceType|String|Plataforma do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: `desktop` , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` `unknown` `cloudPC`  Opcional. Somente leitura.|
|id|String|A identidade exclusiva dessa entidade. Obrigatório. Somente leitura.|
|inGracePeriodUntilDateTime|DateTimeOffset|A data e a hora em que o período de carência expirará. Opcional. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|lastSyncDateTime|DateTimeOffset|A data e a hora em que o dispositivo concluiu pela última vez uma sincronização bem-sucedida com Microsoft Endpoint Manager. Opcional. Somente leitura.|
|managedDeviceId|String|O identificador do dispositivo gerenciado no Microsoft Endpoint Manager. Opcional. Somente leitura.|
|managedDeviceName|String|O nome de exibição do dispositivo gerenciado. Opcional. Somente leitura.|
|fabricante|String|A fabricação do dispositivo. Opcional. Somente leitura.|
|modelo|String|O modelo do dispositivo. Opcional. Somente leitura.|
|osDescription|Cadeia de caracteres|A descrição do sistema operacional do dispositivo gerenciado. Opcional. Somente leitura.|
|osVersion|String|A versão do sistema operacional para o dispositivo gerenciado. Opcional. Somente leitura.|
|ownerType|String|O tipo de proprietário do dispositivo gerenciado. Opcional. Somente leitura.|
|tenantDisplayName|String|O nome de exibição do locatário gerenciado. Opcional. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceCompliance",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "complianceStatus": "String",
  "osDescription": "String",
  "osVersion": "String",
  "lastSyncDateTime": "String (timestamp)",
  "ownerType": "String",
  "model": "String",
  "manufacturer": "String",
  "inGracePeriodUntilDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)",
  "deviceType": "String"
}
```
