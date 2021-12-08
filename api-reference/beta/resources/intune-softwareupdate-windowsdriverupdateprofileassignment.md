---
title: Tipo de recurso windowsDriverUpdateProfileAssignment
description: Essa entidade contém as propriedades usadas para atribuir um perfil de atualização de driver do Windows a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f52b955dabdf87230afb939c96da806024aa25e9
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338936"
---
# <a name="windowsdriverupdateprofileassignment-resource-type"></a>Tipo de recurso windowsDriverUpdateProfileAssignment

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa entidade contém as propriedades usadas para atribuir um perfil de atualização de driver do Windows a um grupo.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDriverUpdateProfileAssignments](../api/intune-softwareupdate-windowsdriverupdateprofileassignment-list.md)|[Coleção windowsDriverUpdateProfileAssignment](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|Listar propriedades e relações dos [objetos windowsDriverUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|
|[Obter windowsDriverUpdateProfileAssignment](../api/intune-softwareupdate-windowsdriverupdateprofileassignment-get.md)|[windowsDriverUpdateProfileAssignment](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|Leia propriedades e relações do [objeto windowsDriverUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|
|[Criar windowsDriverUpdateProfileAssignment](../api/intune-softwareupdate-windowsdriverupdateprofileassignment-create.md)|[windowsDriverUpdateProfileAssignment](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|Crie um novo [objeto windowsDriverUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|
|[Excluir windowsDriverUpdateProfileAssignment](../api/intune-softwareupdate-windowsdriverupdateprofileassignment-delete.md)|Nenhum|Exclui um [windowsDriverUpdateProfileAssignment](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md).|
|[Atualizar windowsDriverUpdateProfileAssignment](../api/intune-softwareupdate-windowsdriverupdateprofileassignment-update.md)|[windowsDriverUpdateProfileAssignment](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|Atualize as propriedades de um [objeto windowsDriverUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O Identificador da entidade|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino de atribuição ao que o perfil de atualização de driver é atribuído.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDriverUpdateProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




