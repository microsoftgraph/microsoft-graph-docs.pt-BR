---
title: tipo de recurso de intuneBrandingProfileAssignment
description: Essa entidade contém as propriedades usadas para atribuir um perfil de marcação para um grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcc0b625bc3918206a1d75ae7ef123484ae0357c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431253"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>tipo de recurso de intuneBrandingProfileAssignment

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Essa entidade contém as propriedades usadas para atribuir um perfil de marcação para um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista intuneBrandingProfileAssignments](../api/intune-wip-intunebrandingprofileassignment-list.md)|coleção [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Lista as propriedades e os relacionamentos dos objetos [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Obter intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Leia as propriedades e os relacionamentos do objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Criar intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Crie um novo objeto de [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Excluir intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-delete.md)|Nenhum|Exclui um [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).|
|[Atualizar intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Atualize as propriedades de um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Destino de atribuição atribuída à marcação perfil.|

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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




