---
title: Tipo de recurso deviceManagementScriptUserState
description: Contém propriedades para o estado de executar do usuário do script de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac1ada80cac67de4c2461d4c747e0fe059ea6ef126e11f73d28a940141764578
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145317"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>Tipo de recurso deviceManagementScriptUserState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de executar do usuário do script de gerenciamento de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementScriptUserStates](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[Coleção deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Listar propriedades e relações dos [objetos deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)|
|[Obter deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Ler propriedades e relações do [objeto deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)|
|[Criar deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Crie um novo [objeto deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)|
|[Excluir deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|Nenhum|Exclui um [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).|
|[Atualizar deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Atualize as propriedades de [um objeto deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de estado do usuário do script de gerenciamento de dispositivo. Essa propriedade é somente leitura.|
|successDeviceCount|Int32|Contagem de dispositivos de sucesso para usuários específicos.|
|errorDeviceCount|Int32|Contagem de dispositivos de erro para usuário específico.|
|userPrincipalName|Cadeia de caracteres|Nome de princípio do usuário de usuário específico.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceRunStates|[Coleção deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lista de estados de executar para esse script em todos os dispositivos de usuário específico.|

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




