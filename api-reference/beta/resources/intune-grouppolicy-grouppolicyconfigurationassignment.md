---
title: tipo de recurso groupPolicyConfigurationAssignment
description: A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6fcd7ace912075189ec3e9b5a817181dd392a5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780389"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a>tipo de recurso groupPolicyConfigurationAssignment

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyConfigurationAssignments](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Listar Propriedades e relações dos objetos [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|
|[Obter groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Leia as propriedades e as relações do objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|
|[Criar groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Criar um novo objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|
|[Excluir groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|Nenhum|Exclui [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).|
|[Atualizar groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Atualiza as propriedades de um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O tipo de grupo de destino da configuração da política de grupo.|

## <a name="relationships"></a>Relações
Nenhuma

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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





