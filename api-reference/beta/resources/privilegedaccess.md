---
title: Tipo de recurso privilegedAccess
description: " por exemplo, representa `privilegedAccess/azureResources` o PIM gerenciando o acesso privilegiado aos recursos do Azure."
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: f90b76ca24a4bded8c2206a4a5f45ebcfde4d825
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509550"
---
# <a name="privilegedaccess-resource-type"></a>Tipo de recurso privilegedAccess

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo de funcionalidades fornecidas pelo serviço Privileged Identity Management (PIM). Diferentes instâncias de representam `privilegedAccess` diferentes provedores gerenciados pelo PIM; por exemplo, `privilegedAccess/azureResources` representa o PIM gerenciando o acesso privilegiado aos recursos do Azure.


`privilegedAccess` é somente leitura por enquanto. Não `POST`, `PUT`, `PATCH`ou `DELETE` as operações são suportadas no conjunto `privilegedAccess` de entidades.

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----------|:----------|:----------|
|id         |String     |A id do provedor gerenciado pelo PIM.|
|displayName|Cadeia de caracteres     |O nome de exibição do provedor gerenciado pelo PIM.|


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


