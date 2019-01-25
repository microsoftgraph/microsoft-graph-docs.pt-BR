---
title: tipo de recurso de privilegedAccess
description: " Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure."
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512924"
---
# <a name="privilegedaccess-resource-type"></a>tipo de recurso de privilegedAccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo de funcionalidades fornecido pelo serviço de gerenciamento de identidade privilegiado (PIM). Diferentes instâncias do `privilegedAccess` representam os diferentes provedores gerenciados por PIM; Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure.


`privilegedAccess`é somente leitura por enquanto. Não `POST`, `PUT`, `PATCH`, ou `DELETE` operações são compatíveis com o `privilegedAccess` conjunto de entidade.

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----------|:----------|:----------|
|id         |String     |A identificação do provedor gerenciado por PIM.|
|displayName|String     |O nome de exibição do provedor gerenciado por PIM.|


## <a name="relationships"></a>Relacionamento
| Relação   | Tipo                                         |Descrição|
|:---------------|:---------------------------------------------|:----------|
|recursos       |coleção [governanceResource](../resources/governanceresource.md)            |Uma coleção de recursos para o provedor.|
|roleAssignments |coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)|Uma coleção de atribuições de função para o provedor.|
|roleDefinitions |coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)|Uma coleção de definições de função para o provedor.|
|roleAssignmentRequests |coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Uma coleção de solicitações de atribuição de função para o provedor.|
|roleSettings |coleção [governanceRoleSetting](../resources/governancerolesetting.md)|Uma coleção de configurações de função para o provedor.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
