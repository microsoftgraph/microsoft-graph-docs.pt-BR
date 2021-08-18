---
title: Tipo de recurso deviceManagementScriptDeviceState
description: Contém propriedades para o estado de executar dispositivo do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0b1b4dd5a247bb94fefd4063f70cd219c27fd1e55169350db35474caf6b94ac1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150357"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>Tipo de recurso deviceManagementScriptDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de executar dispositivo do script de gerenciamento de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[Coleção deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Listar propriedades e relações dos [objetos deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Obter deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Leia propriedades e relações do [objeto deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Criar deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Crie um novo [objeto deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Excluir deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|Nenhum|Exclui um [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).|
|[Atualizar deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Atualize as propriedades de [um objeto deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de estado do dispositivo de script de gerenciamento de dispositivo. Essa propriedade é somente leitura.|
|runState|[runState](../resources/intune-shared-runstate.md)|Estado da última versão do script de gerenciamento de dispositivos. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|resultMessage|Cadeia de caracteres|Detalhes da saída de execução.|
|lastStateUpdateDateTime|DateTimeOffset|Última hora em que o script de gerenciamento de dispositivos é executado.|
|errorCode|Int32|Código de erro correspondente à execução errônea do script de gerenciamento de dispositivo.|
|errorDescription|Cadeia de caracteres|Descrição de erro correspondente à execução errônea do script de gerenciamento de dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|Os dispositivos gerenciados que executam o script de gerenciamento de dispositivos.|

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




