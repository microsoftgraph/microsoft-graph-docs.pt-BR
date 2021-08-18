---
title: Tipo de recurso groupPolicyConfigurationAssignment
description: A entidade de atribuição de configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5ba827367bd32d676f56b3665e84f802e040686d083cfb7dc28aa937bdf3403c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54172894"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a>Tipo de recurso groupPolicyConfigurationAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de atribuição de configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyConfigurationAssignments](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|[coleção groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Listar propriedades e relações dos [objetos groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|
|[Obter groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Leia propriedades e relações do [objeto groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|
|[Criar groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Crie um novo [objeto groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|
|[Excluir groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|Nenhum|Exclui um [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).|
|[Atualizar groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Atualize as propriedades de [um objeto groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O tipo de grupos direcionados à configuração da política de grupo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
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




