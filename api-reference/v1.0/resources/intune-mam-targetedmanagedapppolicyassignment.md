---
title: tipo de recurso targetedManagedAppPolicyAssignment
description: O tipo de implantação de grupos ou aplicativos.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f0a8386f0cbf2f7c5e12ae540884e05d76e24443
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448267"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a>tipo de recurso targetedManagedAppPolicyAssignment

Namespace: Microsoft. Graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O tipo de implantação de grupos ou aplicativos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar targetedManagedAppPolicyAssignments](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).|
|[Obter targetedManagedAppPolicyAssignment](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Ler propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).|
|[Excluir targetedManagedAppPolicyAssignment](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|Nenhum|Excluir [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).|
|[Atualizar targetedManagedAppPolicyAssignment](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Atualizar as propriedades de um objeto de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Id|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Identificador de implantação de um grupo ou aplicativo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




