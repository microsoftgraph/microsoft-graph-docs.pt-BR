---
title: tipo de recurso deviceManagementScript
description: O Intune fornecerá ao cliente a capacidade de executar os scripts do PowerShell nos dispositivos de ingresso no Azure Active Directory do Windows 10 registrados. O script pode ser executado uma vez ou periodicamente.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e0a3a4bebaa36ef1f2818b6ced6a9836d6ceb8a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538732"
---
# <a name="devicemanagementscript-resource-type"></a>tipo de recurso deviceManagementScript

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de executar os scripts do PowerShell nos dispositivos de ingresso no Azure Active Directory do Windows 10 registrados. O script pode ser executado uma vez ou periodicamente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementScripts](../api/intune-shared-devicemanagementscript-list.md)|coleção [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Listar Propriedades e relações dos objetos [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|[Obter deviceManagementScript](../api/intune-shared-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Leia as propriedades e as relações do objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|[Criar deviceManagementScript](../api/intune-shared-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Criar um novo objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|[Excluir deviceManagementScript](../api/intune-shared-devicemanagementscript-delete.md)|Nenhum|Exclui [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).|
|[Atualizar deviceManagementScript](../api/intune-shared-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Atualiza as propriedades de um objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|**Gerenciamento de dispositivos**|
|[atribuir ação](../api/intune-shared-devicemanagementscript-assign.md)|Nenhuma|Ainda não documentado|
|**Conjunto de políticas**|
|[ação hasPayloadLinks](../api/intune-shared-devicemanagementscript-haspayloadlinks.md)|coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do script de gerenciamento de dispositivo.|
|displayName|Cadeia de caracteres|Nome do script de gerenciamento de dispositivo.|
|description|String|Descrição opcional para o script de gerenciamento de dispositivo.|
|scriptContent|Binária|O conteúdo de script.|
|createdDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booliano|Indica se a assinatura do script precisa ser verificada.|
|fileName|String|Nome do arquivo de script.|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para esta instância de PowerShellScript.|
|runAs32Bit|Booliano|Um valor que indica se o script do PowerShell deve ser executado como 32 bits|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Gerenciamento de dispositivos**|
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
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
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
  "runAs32Bit": true
}
```



