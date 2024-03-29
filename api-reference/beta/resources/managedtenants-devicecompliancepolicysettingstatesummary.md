---
title: Tipo de recurso deviceCompliancePolicySettingStateSummary
description: Representa um resumo dos estados de configuração da política de conformidade do dispositivo para um determinado locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 409e72591a75ee84159fb59d27e061ebbf8ae3a9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61843393"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>Tipo de recurso deviceCompliancePolicySettingStateSummary

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo dos estados de configuração da política de conformidade do dispositivo para um determinado locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCompliancePolicySettingStateSummary](../api/managedtenants-managedtenant-list-devicecompliancepolicysettingstatesummary.md)|[coleção microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|Obter uma lista dos [objetos deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) e suas propriedades.|
|[Obter deviceCompliancePolicySettingStateSummary](../api/managedtenants-devicecompliancepolicysettingstatesummary-get.md)|[microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|Leia as propriedades e as relações de um [objeto deviceCompliancePolicySettingStateSummary.](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|conflictDeviceCount|Int32|O número de dispositivos em um estado de conflito. Opcional. Somente leitura.|
|errorDeviceCount|Int32|O número de dispositivos em um estado de erro. Opcional. Somente leitura.|
|failedDeviceCount|Int32|O número de dispositivos em um estado com falha. Opcional. Somente leitura.|
|intuneAccountId|String|O identificador da conta Microsoft Intune. Obrigatório. Somente leitura.|
|intuneSettingId|String|O identificador da configuração do Intune. Opcional. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|notApplicableDeviceCount|Int32|O número de dispositivos em um estado não aplicável. Opcional. Somente leitura.|
|pendingDeviceCount|Int32|O número de dispositivos em um estado pendente. Opcional. Somente leitura.|
|policyType|String|O tipo da política de conformidade do dispositivo. Opcional. Somente leitura.|
|settingName|Cadeia de caracteres|O nome da configuração dentro da política de conformidade do dispositivo. Opcional. Somente leitura.|
|succeededDeviceCount|Int32|O número de dispositivos em um estado bem-sucedido. Opcional. Somente leitura.|
|tenantDisplayName|String|O nome de exibição do locatário gerenciado. Obrigatório. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "conflictDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "intuneAccountId": "String",
  "intuneSettingId": "String",
  "notApplicableDeviceCount": "Integer",
  "pendingDeviceCount": "Integer",
  "policyType": "String",
  "settingName": "String",
  "succeededDeviceCount": "Integer",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
