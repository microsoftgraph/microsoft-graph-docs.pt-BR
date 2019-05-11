---
title: tipo de recurso windowsManagementAppHealthState
description: Entidade de estado de integridade do aplicativo de gerenciamento do Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b443c95b363e926777150013e20bef4bc8bc602d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942168"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>tipo de recurso windowsManagementAppHealthState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade de estado de integridade do aplicativo de gerenciamento do Windows.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|coleção [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Listar Propriedades e relações dos objetos [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Obter windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Leia as propriedades e as relações do objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Criar windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Criar um novo objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Excluir windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|Nenhum|Exclui [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).|
|[Atualizar windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Atualiza as propriedades de um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para o estado de integridade do aplicativo de gerenciamento do Windows|
|HealthState|[HealthState](../resources/intune-devices-healthstate.md)|Estado de integridade do aplicativo de gerenciamento do Windows. Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.|
|installedVersion|Cadeia de caracteres|Versão instalada do aplicativo de gerenciamento do Windows.|
|lastCheckInDateTime|DateTimeOffset|Tempo de check-in do aplicativo de gerenciamento do Windows por último.|
|deviceName|String|Nome do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.|
|deviceOSVersion|Cadeia de caracteres|Versão do Windows 10 so do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.|

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




