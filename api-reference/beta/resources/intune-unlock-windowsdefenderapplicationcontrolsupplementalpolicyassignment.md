---
title: tipo de recurso windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Uma classe que contém as propriedades usadas para atribuição de uma política complementar do WindowsDefenderApplicationControl a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b8b6f5fb0608fc702b085f2ba4185db6738a182f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43317660"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicyassignment-resource-type"></a>tipo de recurso windowsDefenderApplicationControlSupplementalPolicyAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para atribuição de uma política complementar do WindowsDefenderApplicationControl a um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDefenderApplicationControlSupplementalPolicyAssignments](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-list.md)|coleção [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Listar Propriedades e relações dos objetos [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .|
|[Obter windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-get.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Leia as propriedades e as relações do objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .|
|[Criar windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-create.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Criar um novo objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .|
|[Excluir windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-delete.md)|None|Exclui [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).|
|[Atualizar windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-update.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Atualiza as propriedades de um objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|A atribuição do grupo de destino definida pelo administrador.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



