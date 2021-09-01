---
title: Tipo de recurso deviceHealthScriptDeviceState
description: Contém propriedades para o estado de executar o dispositivo do script de saúde do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dfdf8398f9551a68a450d053060959f92463779c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793821"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a>Tipo de recurso deviceHealthScriptDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de executar o dispositivo do script de saúde do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceHealthScriptDeviceStates](../api/intune-devices-devicehealthscriptdevicestate-list.md)|[Coleção deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Listar propriedades e relações dos [objetos deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Obter deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Leia propriedades e relações do [objeto deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Criar deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Crie um novo [objeto deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Excluir deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|Nenhum(a)|Exclui um [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).|
|[Atualizar deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Atualize as propriedades de [um objeto deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de estado do dispositivo de script de saúde do dispositivo. Essa propriedade é somente leitura.|
|detectionState|[runState](../resources/intune-devices-runstate.md)|Estado de detecção da última execução de script de saúde do dispositivo. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|O último período de data/hora de quando o script de saúde do dispositivo foi executado|
|expectedStateUpdateDateTime|DateTimeOffset|O próximo horário de quando o script de saúde do dispositivo deve ser executado|
|lastSyncDateTime|DateTimeOffset|A última vez que a Extensão de Managment do Intune foi sincronizada com o Intune|
|preRemediationDetectionScriptOutput|Cadeia de caracteres|Saída do script de detecção antes da correção|
|preRemediationDetectionScriptError|Cadeia de caracteres|Erro do script de detecção antes da correção|
|remediationScriptError|Cadeia de caracteres|Saída de erro do script de correção|
|postRemediationDetectionScriptOutput|Cadeia de caracteres|Saída de script de detecção após correção|
|postRemediationDetectionScriptError|Cadeia de caracteres|Erro do script de detecção após a correção|
|remediationState|[remediationState](../resources/intune-devices-remediationstate.md)|Estado de correção da última execução do script de saúde do dispositivo. Os valores possíveis são: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|
|assignmentFilterIds|Coleção de cadeias de caracteres|Uma lista das IDs de filtro de atribuição usadas para avaliação de aplicabilidade do script de saúde|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|O dispositivo gerenciado no qual o script de saúde do dispositivo foi executado|

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
  "remediationState": "String",
  "assignmentFilterIds": [
    "String"
  ]
}
```



