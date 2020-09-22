---
title: tipo de recurso deviceComplianceScriptDeviceState
description: Contém propriedades para o estado de execução do dispositivo do script de conformidade do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0b1771c752b804aca270b6dc8f31687ca8007904
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060542"
---
# <a name="devicecompliancescriptdevicestate-resource-type"></a>tipo de recurso deviceComplianceScriptDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de execução do dispositivo do script de conformidade do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceComplianceScriptDeviceStates](../api/intune-devices-devicecompliancescriptdevicestate-list.md)|coleção [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Listar Propriedades e relações dos objetos [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) .|
|[Obter deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-get.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Leia as propriedades e as relações do objeto [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) .|
|[Criar deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-create.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Criar um novo objeto [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) .|
|[Excluir deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-delete.md)|Nenhum|Exclui [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).|
|[Atualizar deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-update.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Atualiza as propriedades de um objeto [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de estado do dispositivo de script de conformidade do dispositivo. Essa propriedade é somente leitura.|
|detecçaostate|[runState](../resources/intune-shared-runstate.md)|Estado de detecção da execução do script de conformidade do dispositivo mais recente. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|O último carimbo de data/hora de quando o script de conformidade do dispositivo foi executado|
|expectedStateUpdateDateTime|DateTimeOffset|O carimbo de data/hora seguinte de quando o script de conformidade do dispositivo deve ser executado|
|lastSyncDateTime|DateTimeOffset|A última vez em que a extensão de gerenciamento do Intune foi sincronizada com o Intune|
|scriptOutput|Cadeia de caracteres|Saída do script de detecção|
|scriptError|Cadeia de caracteres|Erro do script de detecção|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|O dispositivo gerenciado no qual o script de conformidade do dispositivo foi executado|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "id": "String (identifier)",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "scriptOutput": "String",
  "scriptError": "String"
}
```






