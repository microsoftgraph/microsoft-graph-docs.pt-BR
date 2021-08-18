---
title: Tipo de recurso policySetAssignment
description: Uma classe que contém as propriedades usadas para a atribuição PolicySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ed8f6cde042a4200203918fe81c29ada714e28a4a8a989243331ea50b5f3f83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239116"
---
# <a name="policysetassignment-resource-type"></a>Tipo de recurso policySetAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a atribuição PolicySet.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar policySetAssignments](../api/intune-policyset-policysetassignment-list.md)|[Coleção policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Listar propriedades e relações dos [objetos policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Obter policySetAssignment](../api/intune-policyset-policysetassignment-get.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Leia propriedades e relações do [objeto policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Criar policySetAssignment](../api/intune-policyset-policysetassignment-create.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Crie um novo [objeto policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Excluir policySetAssignment](../api/intune-policyset-policysetassignment-delete.md)|Nenhum|Exclui um [policySetAssignment](../resources/intune-policyset-policysetassignment.md).|
|[Atualizar policySetAssignment](../api/intune-policyset-policysetassignment-update.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Atualize as propriedades de [um objeto policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do PolicySetAssignment.|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação do PolicySetAssignment.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O grupo de destino de PolicySetAssignment|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




