---
title: tipo de recurso deviceHealthScript
description: O Intune fornecerá ao cliente a capacidade de executar os scripts do PowerShell nos dispositivos de ingresso no Azure Active Directory do Windows 10 registrados. O script pode ser executado uma vez ou periodicamente.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6ad5fc4e12eeb28acbb6e4c0e0cbe085852feda3
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196956"
---
# <a name="devicehealthscript-resource-type"></a>tipo de recurso deviceHealthScript

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de executar os scripts do PowerShell nos dispositivos de ingresso no Azure Active Directory do Windows 10 registrados. O script pode ser executado uma vez ou periodicamente.


Herda de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceHealthScripts](../api/intune-devices-devicehealthscript-list.md)|coleção [deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Listar Propriedades e relações dos objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Obter deviceHealthScript](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Leia as propriedades e as relações do objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Criar deviceHealthScript](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Criar um novo objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Excluir deviceHealthScript](../api/intune-devices-devicehealthscript-delete.md)|Nenhum|Exclui [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).|
|[Atualizar deviceHealthScript](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Atualiza as propriedades de um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do script de gerenciamento de dispositivo. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|displayName|String|Nome do script de gerenciamento de dispositivo. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|descrição|String|Descrição opcional para o script de gerenciamento de dispositivo. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|O intervalo de execução do script. Se não definido, o script será executado uma vez herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|scriptContent|Binária|O conteúdo de script. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi criado. Essa propriedade é somente leitura. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez. Essa propriedade é somente leitura. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md). Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booliano|Indica se a assinatura do script precisa ser verificada. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|fileName|String|Nome do arquivo de script. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para esta instância de PowerShellScript. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|runAs32Bit|Booliano|Um valor que indica se o script do PowerShell deve ser executado como 32 bits herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|complianceRule|[deviceHealthScriptComplianceRule](../resources/intune-devices-devicehealthscriptcompliancerule.md)|Ainda não documentado|
|remediationScriptContent|Binária|Ainda não documentado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivo. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|assignments|coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivo. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Execute o resumo do script de gerenciamento de dispositivos. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|deviceRunStates|coleção [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lista de Estados de execução para este script em todos os dispositivos. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|userRunStates|coleção [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Lista de Estados de execução para este script em todos os usuários. Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "String",
    "operator": "String",
    "detectionValue": "String"
  },
  "remediationScriptContent": "binary"
}
```



