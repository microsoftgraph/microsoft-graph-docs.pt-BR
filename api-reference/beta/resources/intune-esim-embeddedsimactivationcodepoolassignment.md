---
title: Tipo de recurso embeddedSIMActivationCodePoolAssignment
description: A entidade de atribuição de pool de código de ativação de SIM incorporada atribui um ESPECÍFICO embeddedSIMActivationCodePool a um grupo de dispositivos AAD.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b85c5af3298dc12b868041deb923b3fbda79c208
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789569"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a>Tipo de recurso embeddedSIMActivationCodePoolAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de atribuição de pool de código de ativação de SIM incorporada atribui um ESPECÍFICO embeddedSIMActivationCodePool a um grupo de dispositivos AAD.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar embeddedSIMActivationCodePoolAssignments](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|[Coleção embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Listar propriedades e relações dos [objetos embeddedSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|
|[Obter embeddedSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Leia propriedades e relações do [objeto embeddedSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|
|[Criar embeddedSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Crie um novo [objeto embeddedSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|
|[Excluir embeddedSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|Nenhum(a)|Exclui um [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).|
|[Atualizar embeddedSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Atualize as propriedades de [um objeto EMBEDDEDSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) incorporado.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a atribuição do pool de código de ativação do SIM incorporado. Valor gerado pelo sistema atribuído quando criado.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O tipo de grupos direcionados pelo pool de código de ativação do SIM incorporado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePoolAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



