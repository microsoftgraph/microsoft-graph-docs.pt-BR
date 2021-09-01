---
title: Tipo de recurso deviceShellScript
description: O Intune fornecerá ao cliente a capacidade de executar seus scripts do Shell nos dispositivos Mac OS inscritos. O script pode ser executado uma vez ou periodicamente.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1615cf8e8292f39c13bfd019e71803dd86303c2c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785119"
---
# <a name="deviceshellscript-resource-type"></a>Tipo de recurso deviceShellScript

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de executar seus scripts do Shell nos dispositivos Mac OS inscritos. O script pode ser executado uma vez ou periodicamente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceShellScripts](../api/intune-devices-deviceshellscript-list.md)|[Coleção deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Listar propriedades e relações dos objetos [deviceShellScript.](../resources/intune-devices-deviceshellscript.md)|
|[Obter deviceShellScript](../api/intune-devices-deviceshellscript-get.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Leia propriedades e relações do [objeto deviceShellScript.](../resources/intune-devices-deviceshellscript.md)|
|[Criar deviceShellScript](../api/intune-devices-deviceshellscript-create.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Crie um novo [objeto deviceShellScript.](../resources/intune-devices-deviceshellscript.md)|
|[Excluir deviceShellScript](../api/intune-devices-deviceshellscript-delete.md)|Nenhum(a)|Exclui um [deviceShellScript](../resources/intune-devices-deviceshellscript.md).|
|[Atualizar deviceShellScript](../api/intune-devices-deviceshellscript-update.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Atualize as propriedades de um [objeto deviceShellScript.](../resources/intune-devices-deviceshellscript.md)|
|[atribuir ação](../api/intune-devices-deviceshellscript-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|executionFrequency|Duration|O intervalo para que o script seja executado. Se não estiver definido, o script será executado uma vez|
|retryCount|Int32|Número de vezes em que o script será retridido se ele falhar|
|blockExecutionNotifications|Boleano|Não notifica ao usuário que um script está sendo executado|
|id|Cadeia de caracteres|Identificador exclusivo do script de gerenciamento de dispositivos.|
|displayName|Cadeia de caracteres|Nome do script de gerenciamento de dispositivos.|
|descrição|Cadeia de caracteres|Descrição opcional para o script de gerenciamento de dispositivos.|
|scriptContent|Binário|O conteúdo do script.|
|createdDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivos foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivos foi modificado pela última vez. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|fileName|String|Nome do arquivo de script.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para esta instância do PowerShellScript.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivos.|
|assignments|[Coleção deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivos.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Execute o resumo do script de gerenciamento de dispositivos.|
|deviceRunStates|[Coleção deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lista de estados de executar para esse script em todos os dispositivos.|
|userRunStates|[Coleção deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Lista de estados de executar para esse script em todos os usuários.|

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



