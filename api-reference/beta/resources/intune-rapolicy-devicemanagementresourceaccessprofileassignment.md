---
title: Tipo de recurso deviceManagementResourceAccessProfileAssignment
description: Entidade que descreve configurações de nível de locatário para credenciais derivadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 608e63b6b41ef6cc8f6a0f9b45d3aec2d00316a6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806583"
---
# <a name="devicemanagementresourceaccessprofileassignment-resource-type"></a>Tipo de recurso deviceManagementResourceAccessProfileAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que descreve configurações de nível de locatário para credenciais derivadas

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementResourceAccessProfileAssignments](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-list.md)|[Coleção deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Listar propriedades e relações dos [objetos deviceManagementResourceAccessProfileAssignment.](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|
|[Obter deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-get.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Leia propriedades e relações do [objeto deviceManagementResourceAccessProfileAssignment.](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|
|[Criar deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-create.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Crie um novo [objeto deviceManagementResourceAccessProfileAssignment.](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|
|[Excluir deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-delete.md)|Nenhum(a)|Exclui um [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).|
|[Atualizar deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-update.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Atualize as propriedades de [um objeto deviceManagementResourceAccessProfileAssignment.](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para as atribuições|
|finalidade|[deviceManagementResourceAccessProfileIntent](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|A intenção de atribuição para o perfil de acesso ao recurso. Os valores possíveis são: `apply` e `remove`.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino de atribuição para o perfil de acesso ao recurso.|
|sourceId|Cadeia de caracteres|O identificador da origem da atribuição.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementResourceAccessProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "sourceId": "String"
}
```



