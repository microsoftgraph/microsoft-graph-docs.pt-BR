---
title: Tipo de recurso windowsProtectionState
description: Representa o estado Windows proteção para dispositivos gerenciados que executam Windows.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: dc89db998f8fa75e46b3346f2517e5ee950e0ab5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401971"
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
|antiMalwareVersion|Cadeia de caracteres|A versão anti-malware para o dispositivo gerenciado. Opcional. Somente leitura.|
|attentionRequired|Boolean|Um sinalizador indicando se a atenção é necessária para o dispositivo gerenciado. Opcional. Somente leitura.|
|deviceDeleted|Boolean|Um sinalizador indicando se o dispositivo gerenciado foi excluído. Opcional. Somente leitura.|
|devicePropertyRefreshDateTime|DateTimeOffset|A data e a hora em que a propriedade do dispositivo foi atualizada. Opcional. Somente leitura.|
|engineVersion|Cadeia de caracteres|A versão do mecanismo antivírus para o dispositivo gerenciado. Opcional. Somente leitura.|
|fullScanOverdue|Boolean|Um sinalizador indicando se a verificação rápida está atrasada para o dispositivo gerenciado. Opcional. Somente leitura.|
|fullScanRequired|Boolean|Um sinalizador indicando se a verificação completa está atrasada para o dispositivo gerenciado. Opcional. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo para o estado Windows proteção. Obrigatório. Somente leitura.|
|lastFullScanDateTime|DateTimeOffset|A data e a hora em que uma verificação completa foi concluída. Opcional. Somente leitura.|
|lastFullScanSignatureVersion|Cadeia de caracteres|A versão anti-malware usada para executar a última verificação completa. Opcional. Somente leitura.|
|lastQuickScanDateTime|DateTimeOffset|A data e a hora em que uma verificação rápida foi concluída. Opcional. Somente leitura.|
|lastQuickScanSignatureVersion|Cadeia de caracteres|A versão anti-malware usada para executar a última verificação completa. Opcional. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|lastReportedDateTime|DateTimeOffset|A data e a hora em que o estado de proteção foi relatado pela última vez para o dispositivo gerenciado. Opcional. Somente leitura.|
|malwareProtectionEnabled|Boolean|Um sinalizador indicando se a proteção contra malware está habilitada para o dispositivo gerenciado. Opcional. Somente leitura.|
|managedDeviceHealthState|Cadeia de caracteres|O estado de saúde do dispositivo gerenciado. Opcional. Somente leitura.|
|managedDeviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo gerenciado. Opcional. Somente leitura.|
|managedDeviceName|String|O nome de exibição do dispositivo gerenciado. Opcional. Somente leitura.|
|networkInspectionSystemEnabled|Boolean|Um sinalizador indicando se o sistema de inspeção de rede está habilitado. Opcional. Somente leitura.|
|quickScanOverdue|Boolean|Um sinalizador indicando o clima em que uma verificação rápida está atrasada. Opcional. Somente leitura.|
|realTimeProtectionEnabled|Boolean|Um sinalizador indicando se a proteção em tempo real está habilitada. Opcional. Somente leitura.|
|rebootRequired|Boolean|Um sinalizador indicando se uma reinicialização é necessária. Opcional. Somente leitura.|
|signatureUpdateOverdue|Boolean|Um sinalizador indicando se uma atualização de assinatura está atrasada. Opcional. Somente leitura.|
|signatureVersion|Cadeia de caracteres|A versão de assinatura do dispositivo gerenciado. Opcional. Somente leitura.|
|tenantDisplayName|Cadeia de caracteres|O nome de exibição do locatário gerenciado. Opcional. Somente leitura.|
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
