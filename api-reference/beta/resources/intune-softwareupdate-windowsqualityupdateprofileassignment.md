---
title: Tipo de recurso windowsQualityUpdateProfileAssignment
description: Essa entidade contém as propriedades usadas para atribuir um perfil de atualização de qualidade do Windows a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 875ce2dc0ab7da6308a8163ac0652200d4c370c7
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346693"
---
# <a name="windowsqualityupdateprofileassignment-resource-type"></a>Tipo de recurso windowsQualityUpdateProfileAssignment

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa entidade contém as propriedades usadas para atribuir um perfil de atualização de qualidade do Windows a um grupo.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsQualityUpdateProfileAssignments](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-list.md)|[coleção windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Listar propriedades e relações dos [objetos windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Obter windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-get.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Leia propriedades e relações do [objeto windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Criar windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-create.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Crie um novo [objeto windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Excluir windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-delete.md)|Nenhum|Exclui um [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md).|
|[Atualizar windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-update.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Atualize as propriedades de um [objeto windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O Identificador da entidade|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino de atribuição ao que o perfil de atualização de qualidade é atribuído.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdateProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




