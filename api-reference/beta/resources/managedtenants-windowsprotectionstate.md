---
title: Tipo de recurso windowsProtectionState
description: Representa o estado Windows proteção para dispositivos gerenciados que executam Windows.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d93cc321180ec948865da9a3ef93431f2ac7cb50
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863160"
---
# <a name="windowsprotectionstate-resource-type"></a>Tipo de recurso windowsProtectionState

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado Windows proteção para dispositivos gerenciados que executam Windows.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsProtectionStates](../api/managedtenants-managedtenant-list-windowsprotectionstates.md)|[coleção microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md)|Obter uma lista dos [objetos windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) e suas propriedades.|
|[Obter windowsProtectionState](../api/managedtenants-windowsprotectionstate-get.md)|[microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md)|Leia as propriedades e as relações de um [objeto windowsProtectionState.](../resources/managedtenants-windowsprotectionstate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|antiMalwareVersion|String|A versão anti-malware para o dispositivo gerenciado. Opcional. Somente leitura.|
|attentionRequired|Booliano|Um sinalizador indicando se a atenção é necessária para o dispositivo gerenciado. Opcional. Somente leitura.|
|deviceDeleted|Booliano|Um sinalizador indicando se o dispositivo gerenciado foi excluído. Opcional. Somente leitura.|
|devicePropertyRefreshDateTime|DateTimeOffset|A data e a hora em que a propriedade do dispositivo foi atualizada. Opcional. Somente leitura.|
|engineVersion|String|A versão do mecanismo antivírus para o dispositivo gerenciado. Opcional. Somente leitura.|
|fullScanOverdue|Booliano|Um sinalizador indicando se a verificação rápida está atrasada para o dispositivo gerenciado. Opcional. Somente leitura.|
|fullScanRequired|Booliano|Um sinalizador indicando se a verificação completa está atrasada para o dispositivo gerenciado. Opcional. Somente leitura.|
|id|String|O identificador exclusivo para o estado Windows proteção. Obrigatório. Somente leitura.|
|lastFullScanDateTime|DateTimeOffset|A data e a hora em que uma verificação completa foi concluída. Opcional. Somente leitura.|
|lastFullScanSignatureVersion|String|A versão anti-malware usada para executar a última verificação completa. Opcional. Somente leitura.|
|lastQuickScanDateTime|DateTimeOffset|A data e a hora em que uma verificação rápida foi concluída. Opcional. Somente leitura.|
|lastQuickScanSignatureVersion|String|A versão anti-malware usada para executar a última verificação completa. Opcional. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|lastReportedDateTime|DateTimeOffset|A data e a hora em que o estado de proteção foi relatado pela última vez para o dispositivo gerenciado. Opcional. Somente leitura.|
|malwareProtectionEnabled|Boolean|Um sinalizador indicando se a proteção contra malware está habilitada para o dispositivo gerenciado. Opcional. Somente leitura.|
|managedDeviceHealthState|String|O estado de saúde do dispositivo gerenciado. Opcional. Somente leitura.|
|managedDeviceId|String|O identificador exclusivo do dispositivo gerenciado. Opcional. Somente leitura.|
|managedDeviceName|String|O nome de exibição do dispositivo gerenciado. Opcional. Somente leitura.|
|networkInspectionSystemEnabled|Boolean|Um sinalizador indicando se o sistema de inspeção de rede está habilitado. Opcional. Somente leitura.|
|quickScanOverdue|Booliano|Um sinalizador indicando o clima em que uma verificação rápida está atrasada. Opcional. Somente leitura.|
|realTimeProtectionEnabled|Booliano|Um sinalizador indicando se a proteção em tempo real está habilitada. Opcional. Somente leitura.|
|rebootRequired|Booliano|Um sinalizador indicando se uma reinicialização é necessária. Opcional. Somente leitura.|
|signatureUpdateOverdue|Booliano|Um sinalizador indicando se uma atualização de assinatura está atrasada. Opcional. Somente leitura.|
|signatureVersion|String|A versão de assinatura do dispositivo gerenciado. Opcional. Somente leitura.|
|tenantDisplayName|String|O nome de exibição do locatário gerenciado. Opcional. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.windowsProtectionState",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.windowsProtectionState",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "malwareProtectionEnabled": "Boolean",
  "managedDeviceHealthState": "String",
  "realTimeProtectionEnabled": "Boolean",
  "networkInspectionSystemEnabled": "Boolean",
  "quickScanOverdue": "Boolean",
  "fullScanOverdue": "Boolean",
  "signatureUpdateOverdue": "Boolean",
  "rebootRequired": "Boolean",
  "attentionRequired": "Boolean",
  "fullScanRequired": "Boolean",
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)",
  "devicePropertyRefreshDateTime": "String (timestamp)",
  "deviceDeleted": "Boolean",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
