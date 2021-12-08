---
title: Tipo de recurso hardwareConfigurationAssignment
description: Contém propriedades usadas para atribuir uma configuração de hardware a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ba4a9f20a0f71bbc02f2f91570de56c7f391372
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345378"
---
# <a name="hardwareconfigurationassignment-resource-type"></a>Tipo de recurso hardwareConfigurationAssignment

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir uma configuração de hardware a um grupo.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar hardwareConfigurationAssignments](../api/intune-deviceconfig-hardwareconfigurationassignment-list.md)|[Coleção hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Listar propriedades e relações dos [objetos hardwareConfigurationAssignment.](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|
|[Obter hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-get.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Leia propriedades e relações do [objeto hardwareConfigurationAssignment.](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|
|[Criar hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-create.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Crie um novo [objeto hardwareConfigurationAssignment.](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|
|[Excluir hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-delete.md)|Nenhum|Exclui um [hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md).|
|[Atualizar hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-update.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Atualize as propriedades de um [objeto hardwareConfigurationAssignment.](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de atribuição do grupo de configuração de hardware. Essa propriedade é somente leitura.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|A ID do grupo Azure Active Directory que estamos direcionando para a configuração.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




