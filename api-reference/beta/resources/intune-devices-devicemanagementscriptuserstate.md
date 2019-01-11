---
title: tipo de recurso de deviceManagementScriptUserState
description: Contém propriedades para o usuário executada no estado do script de gerenciamento de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bf355a6ab2c217fa802288f6d2f4f062a3c47f4b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806024"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>tipo de recurso de deviceManagementScriptUserState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades para o usuário executada no estado do script de gerenciamento de dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista deviceManagementScriptUserStates](../api/intune-devices-devicemanagementscriptuserstate-list.md)|coleção [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Lista as propriedades e os relacionamentos dos objetos [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .|
|[Obter deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Leia as propriedades e os relacionamentos do objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .|
|[Criar deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Crie um novo objeto de [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .|
|[Excluir deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|Nenhum|Exclui um [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).|
|[Atualizar deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Atualize as propriedades de um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de estado de usuário de script para gerenciamento do dispositivo.|
|successDeviceCount|Int32|Contagem de dispositivo de sucesso para usuário específico.|
|errorDeviceCount|Int32|Contagem de dispositivo de erro para usuário específico.|
|userPrincipalName|Cadeia de caracteres|Nome do princípio de usuário do usuário específico.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceRunStates|coleção [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lista de estados de execução para esse script em todos os dispositivos de usuário específico.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "userPrincipalName": "String"
}
```





