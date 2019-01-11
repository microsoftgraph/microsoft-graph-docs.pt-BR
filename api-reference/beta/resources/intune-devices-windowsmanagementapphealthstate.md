---
title: tipo de recurso de windowsManagementAppHealthState
description: Entidade de estado integridade do aplicativo de gerenciamento de Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 23381aed47ade8f42937f6bc48cfff33b36d1fa7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875296"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>tipo de recurso de windowsManagementAppHealthState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade de estado integridade do aplicativo de gerenciamento de Windows.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|coleção [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Lista as propriedades e os relacionamentos dos objetos [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Obter windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Leia as propriedades e os relacionamentos do objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Criar windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Crie um novo objeto de [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Excluir windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|Nenhum|Exclui um [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).|
|[Atualizar windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Atualize as propriedades de um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para o estado de integridade de aplicativo de gerenciamento do Windows|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Estado de integridade do aplicativo do gerenciamento do Windows. Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.|
|installedVersion|Cadeia de caracteres|Versão instalada do aplicativo de gerenciamento do Windows.|
|lastCheckInDateTime|DateTimeOffset|Aplicativo de gerenciamento do Windows hora do último check-in.|
|deviceName|Cadeia de caracteres|Nome do dispositivo no qual o Windows o aplicativo de gerenciamento está instalado.|
|deviceOSVersion|Cadeia de caracteres|Versão do sistema operacional do Windows 10 do dispositivo no qual o Windows o aplicativo de gerenciamento está instalado.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```





