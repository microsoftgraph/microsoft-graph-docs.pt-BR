---
title: tipo de recurso Entidadegovernanceresource
description: Representa os recursos que podem ser gerenciados pelo gerenciamento de identidade privilegiado (PIM). Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso como uma máquina virtual, um banco de dados SQL, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 4cfc4232fccf5c68649223746fdad853883166b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058380"
---
# <a name="governanceresource-resource-type"></a>tipo de recurso Entidadegovernanceresource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os recursos que podem ser gerenciados pelo gerenciamento de identidade privilegiado (PIM). Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso como uma máquina virtual, um banco de dados SQL, etc.


## <a name="methods"></a>Methods

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | coleção [entidadegovernanceresource](../resources/governanceresource.md)|Lista uma coleção de recursos aos quais o solicitante tem acesso.|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Leia as propriedades e as relações de uma entidade de recurso especificada por ID.|
|[Registrar](../api/governanceresource-register.md) | |Registre uma assinatura do Azure ou um grupo de gerenciamento não gerenciados no serviço PIM. |

Não `POST` , `PUT` , `PATCH` , `DELETE` há suporte no `roleDefinitions` conjunto de entidades por enquanto.

## <a name="properties"></a>Propriedades
| Propriedade          |Tipo         |Descrição|
|:------------------|:----------|:----------|
|id                 |String     |A ID do recurso. Está no formato GUID.|
|externalId           |Cadeia de caracteres   |A ID externa do recurso, que representa sua ID original no sistema externo. Por exemplo, a ID externa de um recurso de assinatura pode ser "/subscriptions/c14ae696-5e0c-4E5D-88cc-bef6637737ac". |
|tipo               |String     |Obrigatório. Tipo de recurso. Por exemplo, para recursos do Azure, o tipo poderia ser "Subscription", "resourcer", "Microsoft. SQL/Server", etc.|
|displayName        |String     |O nome de exibição do recurso.|
|status             |String     |O status de um determinado recurso. Por exemplo, ele pode representar se o recurso está bloqueado ou não (valores: `Active` / `Locked` ). Observação: essa propriedade pode ser estendida no futuro para dar suporte a mais cenários.|
|registeredDateTime|DateTimeOffset      |Representa a data e hora em que o recurso é registrado no PIM.|
|registeredRoot|String      |ExternalId do escopo raiz do recurso que é registrado no PIM. O escopo raiz pode ser os recursos pai, avô ou ancestral superior.|
|roleAssignmentCount|Int32      |Opcional. O número de atribuições de função para determinado recurso. Para obter a propriedade, explictly use `$select=roleAssignmentCount` na consulta.|
|roleDefinitionCount|Int32      |Opcional. O número de definições de função para o recurso especificado. Para obter a propriedade, explictly use `$select=roleDefinitionCount` na consulta.|
|permissões|[governancePermission](../resources/governancepermission.md)      |Opcional. Ele representa o status do acesso do solicitante ao recurso. Para obter a propriedade, explictly use `$select=permissions` na consulta.|

## <a name="relationships"></a>Relações
| Relação   | Tipo                                         |Descrição|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)|A coleção de atribuições de função para o recurso.|
|roleDefinitions |coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)|O conjunto de defintions de função para o recurso.|
|roleAssignmentRequests |coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|A coleção de solicitações de atribuição de função para o recurso.|
|roleSettings |coleção [governanceRoleSetting](../resources/governancerolesetting.md)|O conjunto de configurações de função para o recurso.|
|primário          |[governanceResource](../resources/governanceresource.md)           |Apenas leitura. O recurso pai. para o `pimforazurerbac` cenário, ele pode representar a assinatura à qual o recurso pertence.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String",
  "roleAssignmentCount": 12356,
  "roleDefinitionCount": 12356,
  "permissions": {
    "@odata.type": "microsoft.graph.governancePermission"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


