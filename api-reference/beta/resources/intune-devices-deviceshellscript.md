---
title: tipo de recurso deviceShellScript
description: O Intune fornecerá ao cliente a capacidade de executar os scripts do Shell nos dispositivos do Mac OS registrados. O script pode ser executado uma vez ou periodicamente.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f6f1fd1f5a543a3caa3e0fcbf53272ea12d4c572
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034787"
---
# <a name="deviceshellscript-resource-type"></a>tipo de recurso deviceShellScript

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de executar os scripts do Shell nos dispositivos do Mac OS registrados. O script pode ser executado uma vez ou periodicamente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceShellScripts](../api/intune-devices-deviceshellscript-list.md)|coleção [deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Listar Propriedades e relações dos objetos [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .|
|[Obter deviceShellScript](../api/intune-devices-deviceshellscript-get.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Leia as propriedades e as relações do objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .|
|[Criar deviceShellScript](../api/intune-devices-deviceshellscript-create.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Criar um novo objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .|
|[Excluir deviceShellScript](../api/intune-devices-deviceshellscript-delete.md)|Nenhum|Exclui [deviceShellScript](../resources/intune-devices-deviceshellscript.md).|
|[Atualizar deviceShellScript](../api/intune-devices-deviceshellscript-update.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Atualiza as propriedades de um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .|
|[atribuir ação](../api/intune-devices-deviceshellscript-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|executionFrequency|Duração|O intervalo de execução do script. Se não definido, o script é executado uma vez.|
|retryCount|Int32|O número de vezes que o script deve ser repetido se falhar.|
|blockExecutionNotifications|Booliano|Indica se o usuário é notificado quando um script é executado.|
|id|String|Identificador exclusivo do script de gerenciamento de dispositivo.|
|displayName|Cadeia de caracteres|O nome do script de gerenciamento de dispositivo.|
|description|String|Descrição opcional para o script de gerenciamento de dispositivo.|
|scriptContent|Binária|O conteúdo de script.|
|createdDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|fileName|String|O nome do arquivo de script.|
|roleScopeTagIds|String collection|A lista de IDs de marca de escopo para esta instância de PowerShellScript.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivo.|
|assignments|coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivo.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Execute o resumo do script de gerenciamento de dispositivos.|
|deviceRunStates|coleção [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lista de Estados de execução para este script em todos os dispositivos.|
|userRunStates|coleção [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Lista de Estados de execução para este script em todos os usuários.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceShellScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "String (duration)",
  "retryCount": 1024,
  "blockExecutionNotifications": true,
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```



