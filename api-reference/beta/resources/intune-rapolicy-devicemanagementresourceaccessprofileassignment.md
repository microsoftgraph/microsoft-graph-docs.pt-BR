---
title: tipo de recurso deviceManagementResourceAccessProfileAssignment
description: Entidade que descreve as configurações de nível de locatário para credenciais derivadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d52845a705cce3ef7a2171b151c014c994cd78a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301608"
---
# <a name="devicemanagementresourceaccessprofileassignment-resource-type"></a>tipo de recurso deviceManagementResourceAccessProfileAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que descreve as configurações de nível de locatário para credenciais derivadas

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementResourceAccessProfileAssignments](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-list.md)|coleção [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Listar Propriedades e relações dos objetos [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .|
|[Obter deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-get.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Leia as propriedades e as relações do objeto [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .|
|[Criar deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-create.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Criar um novo objeto [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .|
|[Excluir deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-delete.md)|Nenhum|Exclui [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).|
|[Atualizar deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-update.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Atualiza as propriedades de um objeto [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo das atribuições|
|finalidade|[deviceManagementResourceAccessProfileIntent](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|A intenção de atribuição para o perfil de acesso do recurso. Os valores possíveis são: `apply` e `remove`.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino da atribuição para o perfil de acesso do recurso.|
|sourceId|String|O identificador da origem da atribuição.|

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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "sourceId": "String"
}
```




