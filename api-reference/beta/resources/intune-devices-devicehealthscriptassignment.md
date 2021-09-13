---
title: Tipo de recurso deviceHealthScriptAssignment
description: Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5ae4954314224db4bd65278e95ed8f0e7a8ec9b8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017384"
---
# <a name="devicehealthscriptassignment-resource-type"></a>Tipo de recurso deviceHealthScriptAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceHealthScriptAssignments](../api/intune-devices-devicehealthscriptassignment-list.md)|[Coleção deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Listar propriedades e relações dos [objetos deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)|
|[Obter deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-get.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Leia propriedades e relações do [objeto deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)|
|[Criar deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-create.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Crie um novo [objeto deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)|
|[Excluir deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-delete.md)|None|Exclui um [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).|
|[Atualizar deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-update.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Atualize as propriedades de um [objeto deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de atribuição de script de saúde do dispositivo. Essa propriedade é somente leitura.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O Azure Active Directory grupo para o que estamos direcionando o script|
|runRemediationScript|Boolean|Determinar se queremos executar somente script de detecção ou executar script de detecção e script de correção|
|runSchedule|[deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|Agenda de executar scripts para o grupo de destino|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
    "interval": 1024,
    "useUtc": true,
    "time": "String (time of day)"
  }
}
```



