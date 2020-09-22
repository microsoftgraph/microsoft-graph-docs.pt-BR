---
title: tipo de recurso deviceHealthScriptDeviceState
description: Contém propriedades para o estado de execução do dispositivo do script de integridade do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 628e48ebd263e2f315ce3868730de91154780061
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060339"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a>tipo de recurso deviceHealthScriptDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de execução do dispositivo do script de integridade do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceHealthScriptDeviceStates](../api/intune-devices-devicehealthscriptdevicestate-list.md)|coleção [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Listar Propriedades e relações dos objetos [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .|
|[Obter deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Leia as propriedades e as relações do objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .|
|[Criar deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Criar um novo objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .|
|[Excluir deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|Nenhum|Exclui [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).|
|[Atualizar deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Atualiza as propriedades de um objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de estado do dispositivo de script de integridade do dispositivo. Essa propriedade é somente leitura.|
|detecçaostate|[runState](../resources/intune-shared-runstate.md)|Estado de detecção da execução do script de integridade do dispositivo mais recente. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|O último carimbo de data/hora de quando o script de integridade do dispositivo é executado|
|expectedStateUpdateDateTime|DateTimeOffset|O carimbo de data/hora seguinte de quando o script de integridade do dispositivo deve ser executado|
|lastSyncDateTime|DateTimeOffset|A última vez em que a extensão de gerenciamento do Intune foi sincronizada com o Intune|
|preRemediationDetectionScriptOutput|Cadeia de caracteres|Saída do script de detecção antes da correção|
|preRemediationDetectionScriptError|Cadeia de caracteres|Erro do script de detecção antes da correção|
|remediationScriptError|Cadeia de caracteres|Saída de erro do script de correção|
|postRemediationDetectionScriptOutput|Cadeia de caracteres|Saída do script de detecção após a correção|
|postRemediationDetectionScriptError|Cadeia de caracteres|Erro do script de detecção após a correção|
|remediationState|[remediationState](../resources/intune-devices-remediationstate.md)|Estado de correção da execução do script de integridade do dispositivo mais recente. Os valores possíveis são: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|O dispositivo gerenciado no qual o script de integridade do dispositivo foi executado|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "String (identifier)",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "preRemediationDetectionScriptError": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String",
  "postRemediationDetectionScriptError": "String",
  "remediationState": "String"
}
```






