---
title: tipo de recurso de privilegedAccess
description: " Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure."
localization_priority: Normal
ms.openlocfilehash: f4166fb539d627730c68c7e039fd8d672ff4c785
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810049"
---
# <a name="privilegedaccess-resource-type"></a>tipo de recurso de privilegedAccess

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um grupo de funcionalidades fornecido pelo serviço de gerenciamento de identidade privilegiado (PIM). Diferentes instâncias do `privilegedAccess` representam os diferentes provedores gerenciados por PIM; Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure.


`privilegedAccess`é somente leitura por enquanto. Não `POST`, `PUT`, `PATCH`, ou `DELETE` operações são compatíveis com o `privilegedAccess` conjunto de entidade.

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----------|:----------|:----------|
|id         |Cadeia de caracteres     |A identificação do provedor gerenciado por PIM.|
|displayName|Cadeia de caracteres     |O nome de exibição do provedor gerenciado por PIM.|


## <a name="relationships"></a>Relações
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
