---
title: Tipo de recurso managedDeviceComplianceTrend
description: Representa uma tendência de dispositivos compatíveis e não compatíveis para um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 70c3c84c5da6ffb2660a6289bc55c6ab3eef64be
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401939"
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
|countDateTime|Cadeia de caracteres|O instantâneo de conformidade de data e hora foi executado. Obrigatório. Somente leitura.|
|errorDeviceCount|Int32|O número de dispositivos com um status de erro. Obrigatório. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|inGracePeriodDeviceCount|Int32|O número de dispositivos que estão em um status de período de carência. Obrigatório. Somente leitura.|
|noncompliantDeviceCount|Int32|O número de dispositivos que estão em um status não compatível. Obrigatório. Somente leitura.|
|tenantDisplayName|Cadeia de caracteres|O nome de exibição do locatário gerenciado. Opcional. Somente leitura.|
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
