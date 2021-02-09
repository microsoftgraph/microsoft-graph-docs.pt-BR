---
title: Tipo de recurso deviceManagementScriptDeviceState
description: Contém propriedades para o estado de executar do dispositivo do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6bcce9f566f9f187bf55b8b201ee9ae29f7b627e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158493"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>Tipo de recurso deviceManagementScriptDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de executar do dispositivo do script de gerenciamento de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[Coleção deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Listar propriedades e relações dos [objetos deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Obter deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Leia as propriedades e as relações do [objeto deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Criar deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Crie um novo [objeto deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Excluir deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|Nenhum(a)|Exclui [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).|
|[Atualizar deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Atualizar as propriedades de um [objeto deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de estado do dispositivo de script de gerenciamento de dispositivo. Essa propriedade é somente leitura.|
|runState|[runState](../resources/intune-shared-runstate.md)|Estado da última versão do script de gerenciamento de dispositivos. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|resultMessage|String|Detalhes da saída de execução.|
|lastStateUpdateDateTime|DateTimeOffset|Última hora em que o script de gerenciamento de dispositivos é executado.|
|errorCode|Int32|Código de erro correspondente à execução errada do script de gerenciamento de dispositivos.|
|errorDescription|Cadeia de caracteres|Descrição do erro correspondente à execução errada do script de gerenciamento de dispositivos.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-shared-manageddevice.md)|Os dispositivos gerenciados que executam o script de gerenciamento de dispositivos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "String (identifier)",
  "runState": "String",
  "resultMessage": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "errorCode": 1024,
  "errorDescription": "String"
}
```




