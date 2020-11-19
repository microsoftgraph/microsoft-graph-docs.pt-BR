---
title: tipo de recurso deviceManagementIntentAssignment
description: Entidade de atribuição de intenções
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f02bd5a6d4c566115ac71c397b1084a09c114f5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275843"
---
# <a name="devicemanagementintentassignment-resource-type"></a>tipo de recurso deviceManagementIntentAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade de atribuição de intenções

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntentAssignments](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|coleção [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Listar Propriedades e relações dos objetos [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .|
|[Obter deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Leia as propriedades e as relações do objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .|
|[Criar deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Criar um novo objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .|
|[Excluir deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|Nenhum|Exclui [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).|
|[Atualizar deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Atualiza as propriedades de um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da atribuição|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino da atribuição|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




