---
title: Tipo de recurso unmanagedDeviceDiscoveryTask
description: Esse tipo derivado de tarefa representa uma lista de dispositivos não-managedos descobertos na rede.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 039075c13db6a1dba3c7789e0be2ba5b7fdf3782
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162198"
---
# <a name="unmanageddevicediscoverytask-resource-type"></a>Tipo de recurso unmanagedDeviceDiscoveryTask

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Esse tipo derivado de tarefa representa uma lista de dispositivos não-managedos descobertos na rede.


Herda de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unmanagedDeviceDiscoveryTasks](../api/intune-partnerintegration-unmanageddevicediscoverytask-list.md)|[Coleção unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|Listar propriedades e relações dos [objetos unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|
|[Obter unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-get.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|Leia as propriedades e as relações do [objeto unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|
|[Criar unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-create.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|Crie um novo [objeto unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|
|[Excluir unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-delete.md)|Nenhum(a)|Exclui [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md).|
|[Atualizar unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-update.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|Atualizar as propriedades de [um objeto unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da entidade. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|String|O nome. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|String|A descrição. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|A data de criação. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|A data de vencimento. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|A categoria. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Os valores possíveis são: `unknown` e `advancedThreatProtection`.|
|prioridade|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|A prioridade. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Os valores possíveis são: `none`, `high`, `low`.|
|criador|String|O endereço de email do criador. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|creatorNotes|String|Observações do criador. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|String|O nome ou email do administrador ao que essa tarefa foi atribuída. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|O status. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.|
|unmanagedDevices|[Coleção unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md)|Dispositivos não-manageados descobertos na rede.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unmanagedDeviceDiscoveryTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "String",
      "osVersion": "String",
      "ipAddress": "String",
      "deviceName": "String",
      "macAddress": "String",
      "domain": "String",
      "manufacturer": "String",
      "model": "String",
      "location": "String",
      "lastLoggedOnUser": "String",
      "lastSeenDateTime": "String (timestamp)"
    }
  ]
}
```




