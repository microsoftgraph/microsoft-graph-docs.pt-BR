---
title: tipo de recurso deviceHealthScriptAssignment
description: Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef7a088f85646d699958b5ebbcbc996b3f0b3d57
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784955"
---
# <a name="devicehealthscriptassignment-resource-type"></a>tipo de recurso deviceHealthScriptAssignment

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceHealthScriptAssignments](../api/intune-devices-devicehealthscriptassignment-list.md)|coleção [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Listar Propriedades e relações dos objetos [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .|
|[Obter deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-get.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Leia as propriedades e as relações do objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .|
|[Criar deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-create.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Criar um novo objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .|
|[Excluir deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-delete.md)|Nenhum|Exclui [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).|
|[Atualizar deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-update.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Atualiza as propriedades de um objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de atribuição de script de integridade do dispositivo. Essa propriedade é somente leitura.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O grupo do Azure Active Directory que estamos direcionando o script para|
|runRemediationScript|Boolean|Determinar se queremos executar somente o script de detecção ou executar o script de detecção e o script de correção|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Agendamento de execução de script para o grupo de destino|

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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  }
}
```



