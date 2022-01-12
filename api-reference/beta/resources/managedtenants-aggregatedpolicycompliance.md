---
title: Tipo de recurso aggregatedPolicyCompliance
description: Representa uma exibição agregada da conformidade do dispositivo para um locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 9db12e1a86ee6953c81be839abee695d2ba3a55a
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862336"
---
# <a name="aggregatedpolicycompliance-resource-type"></a>Tipo de recurso aggregatedPolicyCompliance

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma exibição agregada da conformidade do dispositivo para um locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar aggregatedPolicyCompliances](../api/managedtenants-managedtenant-list-aggregatedpolicycompliances.md)|[coleção microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md)|Obter uma lista dos [objetos aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) e suas propriedades.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|compliancePolicyId|String|Identificador da política de conformidade do dispositivo. Opcional. Somente leitura.|
|compliancePolicyName|String|Nome da política de conformidade do dispositivo. Opcional. Somente leitura.|
|compliancePolicyPlatform|String|Plataforma para a política de conformidade do dispositivo. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidAOSP`, `all`. Opcional. Somente leitura.|
|compliancePolicyType|String|O tipo de política de conformidade. Opcional. Somente leitura.|
|id|String|Identificador exclusivo da política de conformidade do dispositivo agregado. Obrigatório. Somente leitura|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|numberOfCompliantDevices|Int64|O número de dispositivos que estão em um status compatível. Opcional. Somente leitura.|
|numberOfErrorDevices|Int64|O número de dispositivos que estão em um status de erro. Opcional. Somente leitura.|
|numberOfNonCompliantDevices|Int64|O número de dispositivos que estão em um status não compatível. Opcional. Somente leitura.|
|policyModifiedDateTime|DateTimeOffset|A data e a hora em que a política do dispositivo foi modificada pela última vez. Opcional. Somente leitura.|
|tenantDisplayName|String|O nome de exibição do locatário gerenciado. Opcional. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "compliancePolicyId": "String",
  "compliancePolicyName": "String",
  "compliancePolicyType": "String",
  "compliancePolicyPlatform": "String",
  "numberOfCompliantDevices": "Integer",
  "numberOfNonCompliantDevices": "Integer",
  "numberOfErrorDevices": "Integer",
  "policyModifiedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
