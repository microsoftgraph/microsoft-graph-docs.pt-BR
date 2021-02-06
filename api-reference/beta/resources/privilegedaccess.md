---
title: Tipo de recurso privilegedAccess
description: " por exemplo, representa `privilegedAccess/azureResources` o PIM gerenciando o acesso privilegiado aos recursos do Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8a144ba13974a728b4e89fc661f34f20e8157689
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136616"
---
# <a name="privilegedaccess-resource-type"></a>Tipo de recurso privilegedAccess

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo de funcionalidades fornecidas pelo serviço privileged Identity Management (PIM). Diferentes instâncias de representam diferentes provedores gerenciados por PIM; por exemplo, representa o PIM gerenciando o acesso privilegiado `privilegedAccess` `privilegedAccess/azureResources` aos recursos do Azure.


`privilegedAccess` é somente leitura por enquanto. Não `POST` , ou operações são `PUT` `PATCH` `DELETE` suportadas no conjunto de `privilegedAccess` entidades.

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----------|:----------|:----------|
|id         |String     |A id do provedor gerenciado pelo PIM.|
|displayName|String     |O nome de exibição do provedor gerenciado pelo PIM.|


## <a name="relationships"></a>Relações
| Relação   | Tipo                                         |Descrição|
|:---------------|:---------------------------------------------|:----------|
|recursos       |[Coleção governanceResource](../resources/governanceresource.md)            |Uma coleção de recursos para o provedor.|
|roleAssignments |[Coleção governanceRoleAssignment](../resources/governanceroleassignment.md)|Uma coleção de atribuições de função para o provedor.|
|roleDefinitions |[Coleção governanceRoleDefinition](../resources/governanceroledefinition.md)|Uma coleção de definições de função para o provedor.|
|roleAssignmentRequests |[Coleção governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Uma coleção de solicitações de atribuição de função para o provedor.|
|roleSettings |[Coleção governanceRoleSetting](../resources/governancerolesetting.md)|Uma coleção de configurações de função para o provedor.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


