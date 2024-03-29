---
title: Tipo de recurso managedDeviceComplianceTrend
description: Representa uma tendência de dispositivos compatíveis e não compatíveis para um determinado locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 671f54fb20f8ef3ecc94525061009a26e2f583f9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61793891"
---
# <a name="manageddevicecompliancetrend-resource-type"></a>Tipo de recurso managedDeviceComplianceTrend

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma tendência de dispositivos compatíveis e não compatíveis para um determinado locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceComplianceTrends](../api/managedtenants-managedtenant-list-manageddevicecompliancetrends.md)|[Coleção microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)|Obter uma lista dos [objetos managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) e suas propriedades.|
|[Obter managedDeviceComplianceTrend](../api/managedtenants-manageddevicecompliancetrend-get.md)|[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)|Leia as propriedades e as relações de [um objeto managedDeviceComplianceTrend.](../resources/managedtenants-manageddevicecompliancetrend.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|compliantDeviceCount|Int32|O número de dispositivos com um status compatível. Obrigatório. Somente leitura.|
|configManagerDeviceCount|Int32|O número de dispositivos maneados pelo Configuration Manager. Obrigatório. Somente leitura.|
|countDateTime|String|O instantâneo de conformidade de data e hora foi executado. Obrigatório. Somente leitura.|
|errorDeviceCount|Int32|O número de dispositivos com um status de erro. Obrigatório. Somente leitura.|
|id|String|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|inGracePeriodDeviceCount|Int32|O número de dispositivos que estão em um status de período de carência. Obrigatório. Somente leitura.|
|noncompliantDeviceCount|Int32|O número de dispositivos que estão em um status não compatível. Obrigatório. Somente leitura.|
|tenantDisplayName|String|O nome de exibição do locatário gerenciado. Opcional. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Opcional. Somente leitura.|
|unknownDeviceCount|Int32|O número de dispositivos em um status desconhecido. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "unknownDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "noncompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "inGracePeriodDeviceCount": "Integer",
  "configManagerDeviceCount": "Integer",
  "countDateTime": "String"
}
```
