---
title: Tipo de recurso windowsFeatureUpdateProfileAssignment
description: Essa entidade contém as propriedades usadas para atribuir um perfil de atualização de recursos do Windows a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b85aad78cda12df1cdc9eb7b1613c26b5caf53be
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816890"
---
# <a name="windowsfeatureupdateprofileassignment-resource-type"></a>Tipo de recurso windowsFeatureUpdateProfileAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa entidade contém as propriedades usadas para atribuir um perfil de atualização de recursos do Windows a um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsFeatureUpdateProfileAssignments](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-list.md)|[coleção windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Listar propriedades e relações dos [objetos windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|
|[Obter windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-get.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Leia propriedades e relações do [objeto windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|
|[Criar windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-create.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Crie um novo [objeto windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|
|[Excluir windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-delete.md)|Nenhum|Exclui um [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).|
|[Atualizar windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-update.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Atualize as propriedades de um [objeto windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O Identificador da entidade|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino de atribuição ao que o perfil de atualização de recursos é atribuído.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



