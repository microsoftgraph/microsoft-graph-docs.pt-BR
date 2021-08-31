---
title: Tipo de recurso deviceManagementIntentAssignment
description: Entidade de atribuição de intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d74e15f0f1213cd86c35760c814afab4b3326ef
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795189"
---
# <a name="devicemanagementintentassignment-resource-type"></a>Tipo de recurso deviceManagementIntentAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade de atribuição de intenção

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntentAssignments](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|[Coleção deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Listar propriedades e relações dos [objetos deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Obter deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Leia propriedades e relações do [objeto deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Criar deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Crie um novo [objeto deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Excluir deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|Nenhum(a)|Exclui um [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).|
|[Atualizar deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Atualize as propriedades de [um objeto deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da atribuição|
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```



