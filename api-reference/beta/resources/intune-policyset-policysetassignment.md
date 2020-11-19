---
title: tipo de recurso policySetAssignment
description: Uma classe que contém as propriedades usadas para atribuição de Policyset.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51cce7ad66c1374f27c861b1db602ffe6122088c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288023"
---
# <a name="policysetassignment-resource-type"></a>tipo de recurso policySetAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para atribuição de Policyset.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar policySetAssignments](../api/intune-policyset-policysetassignment-list.md)|coleção [policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Listar Propriedades e relações dos objetos [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .|
|[Obter policySetAssignment](../api/intune-policyset-policysetassignment-get.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Leia as propriedades e as relações do objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .|
|[Criar policySetAssignment](../api/intune-policyset-policysetassignment-create.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Criar um novo objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .|
|[Excluir policySetAssignment](../api/intune-policyset-policysetassignment-delete.md)|Nenhum|Exclui [policySetAssignment](../resources/intune-policyset-policysetassignment.md).|
|[Atualizar policySetAssignment](../api/intune-policyset-policysetassignment-update.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Atualiza as propriedades de um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do PolicySetAssignment.|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação do PolicySetAssignment.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O grupo de destino de PolicySetAssignment|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




