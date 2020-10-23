---
title: tipo de recurso intuneBrandingProfileAssignment
description: Esta entidade contém as propriedades usadas para atribuir um perfil de identidade visual a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1815ad30c46b87c687eba7ee09b7f91a5871edd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685405"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>tipo de recurso intuneBrandingProfileAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Esta entidade contém as propriedades usadas para atribuir um perfil de identidade visual a um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar intuneBrandingProfileAssignments](../api/intune-wip-intunebrandingprofileassignment-list.md)|coleção [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Listar Propriedades e relações dos objetos [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Obter intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Leia as propriedades e as relações do objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Criar intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Criar um novo objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Excluir intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-delete.md)|Nenhum|Exclui [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).|
|[Atualizar intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Atualiza as propriedades de um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Destino de atribuição ao qual o perfil de identidade visual está atribuído.|

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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```





