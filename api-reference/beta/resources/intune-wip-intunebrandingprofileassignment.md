---
title: Tipo de recurso intuneBrandingProfileAssignment
description: Essa entidade contém as propriedades usadas para atribuir um perfil de identidade visual a um grupo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01206c92a604a2d38a80dc8f60adb0956ad3d229
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063633"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>Tipo de recurso intuneBrandingProfileAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa entidade contém as propriedades usadas para atribuir um perfil de identidade visual a um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar intuneBrandingProfileAssignments](../api/intune-wip-intunebrandingprofileassignment-list.md)|[Coleção intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Listar propriedades e relações dos objetos [intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)|
|[Obter intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Leia propriedades e relações do [objeto intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)|
|[Criar intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Crie um novo [objeto intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)|
|[Excluir intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-delete.md)|Nenhum|Exclui um [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).|
|[Atualizar intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Atualize as propriedades de um [objeto intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Destino de atribuição ao que o perfil de identidade visual é atribuído.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```



