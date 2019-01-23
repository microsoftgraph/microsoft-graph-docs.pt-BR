---
title: tipo de recurso de deviceManagementScript
description: Intune irá fornecer a capacidade de executar seus scripts do Powershell nos dispositivos windows registrados 10 Azure Active Directory ingressou do cliente. O script pode ser executado uma vez ou periodicamente.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4fda826ec8033cd51ad4dd13dbc5b523a21e9e3a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412524"
---
# <a name="devicemanagementscript-resource-type"></a>tipo de recurso de deviceManagementScript

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Intune irá fornecer a capacidade de executar seus scripts do Powershell nos dispositivos windows registrados 10 Azure Active Directory ingressou do cliente. O script pode ser executado uma vez ou periodicamente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista deviceManagementScripts](../api/intune-devices-devicemanagementscript-list.md)|coleção [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Lista as propriedades e os relacionamentos dos objetos [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Obter deviceManagementScript](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Leia as propriedades e os relacionamentos do objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Criar deviceManagementScript](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Crie um novo objeto de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Excluir deviceManagementScript](../api/intune-devices-devicemanagementscript-delete.md)|Nenhum|Exclui um [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).|
|[Atualizar deviceManagementScript](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Atualize as propriedades de um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Ação assign](../api/intune-devices-devicemanagementscript-assign.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para o script de gerenciamento de dispositivo.|
|displayName|String|Nome do script de gerenciamento de dispositivo.|
|description|String|Descrição opcional para o script de gerenciamento de dispositivo.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|O intervalo de script a ser executado. Se não definido o script será executado uma vez|
|scriptContent|Binária|O conteúdo de script.|
|createdDateTime|DateTimeOffset|A data e hora em que o script de gerenciamento do dispositivo foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que da última modificação o script de gerenciamento de dispositivo.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução em que do script de gerenciamento de dispositivo é executado. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Boolean|Indica se a assinatura de script precisa ser verificada.|
|fileName|String|Nome do arquivo de script.|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para essa instância do PowerShellScript.|
|runAs32Bit|Boolean|Um valor que indica se o script do PowerShell deve ser executado como de 32 bits|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivo.|
|assignments|coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivo.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Execute o resumo de script de gerenciamento de dispositivo.|
|deviceRunStates|coleção [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lista de estados de execução para esse script em todos os dispositivos.|
|userRunStates|coleção [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Lista de estados de execução para esse script entre todos os usuários.|

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




