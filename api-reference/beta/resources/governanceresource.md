---
title: Tipo de recurso governanceResource
description: Representa recursos que podem ser gerenciados por Privileged Identity Management (PIM). Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso, como uma máquina virtual, um banco de dados SQL etc.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 0be4deb0ae3e96ff1c5a19b7d398ff980c2760ae
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397470"
---
# <a name="governanceresource-resource-type"></a>Tipo de recurso governanceResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Representa recursos que podem ser gerenciados por Privileged Identity Management (PIM). Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso, como uma máquina virtual, um banco de dados SQL etc.


## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:----------|
|[Listar](../api/governanceresource-list.md) | [Coleção governanceResource](../resources/governanceresource.md)|Liste uma coleção de recursos aos qual o solicitante tem acesso.|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Ler propriedades e relações de uma entidade de recurso especificada pela ID.|
|[Registrar](../api/governanceresource-register.md) | |Registre uma assinatura ou grupo de gerenciamento não gerenciado do Azure no serviço PIM. |

Não `POST`, `PUT`, `PATCH`têm `DELETE` suporte no conjunto `roleDefinitions` de entidades por enquanto.

## <a name="properties"></a>Propriedades
| Propriedade          |Tipo         |Descrição|
|:------------------|:----------|:----------|
|id                 |Cadeia de caracteres     |A ID do recurso. Ele está no formato GUID.|
|externalId           |Cadeia de caracteres   |A ID externa do recurso, que representa sua ID original no sistema externo. Por exemplo, a ID externa de um recurso de assinatura pode ser "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac". |
|type               |Cadeia de caracteres     |Obrigatório. Tipo de recurso. Por exemplo, para recursos do Azure, o tipo pode ser "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.|
|displayName        |Cadeia de caracteres     |O nome de exibição do recurso.|
|status             |Cadeia de caracteres     |O status de um determinado recurso. Por exemplo, ele pode representar se o recurso está bloqueado ou não (valores: `Active`/`Locked`). Observação: essa propriedade pode ser estendida no futuro para dar suporte a mais cenários.|
|registeredDateTime|DateTimeOffset      |Representa a data em que o recurso é registrado no PIM.|
|registeredRoot|Cadeia de caracteres      |A externalId do escopo raiz do recurso registrado no PIM. O escopo raiz pode ser o pai, avô ou recursos ancestrais superiores.|
|roleAssignmentCount|Int32      |Opcional. O número de atribuições de função para o recurso fornecido. Para obter a propriedade, use explicitamente `$select=roleAssignmentCount` na consulta.|
|roleDefinitionCount|Int32      |Opcional. O número de definições de função para o recurso fornecido. Para obter a propriedade, use explicitamente `$select=roleDefinitionCount` na consulta.|
|permissões|[governancePermission](../resources/governancepermission.md)      |Opcional. Ele representa o status do acesso do solicitante ao recurso. Para obter a propriedade, use explicitamente `$select=permissions` na consulta.|

## <a name="relationships"></a>Relações
| Relação   | Tipo                                         |Descrição|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[coleção governanceRoleAssignment](../resources/governanceroleassignment.md)|A coleção de atribuições de função para o recurso.|
|roleDefinitions |[coleção governanceRoleDefinition](../resources/governanceroledefinition.md)|A coleção de definições de função para o recurso.|
|roleAssignmentRequests |[coleção governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|A coleção de solicitações de atribuição de função para o recurso.|
|roleSettings |[coleção governanceRoleSetting](../resources/governancerolesetting.md)|A coleção de configurações de função para o recurso.|
|primário          |[governanceResource](../resources/governanceresource.md)           |Somente leitura. O recurso pai. para `pimforazurerbac` o cenário, ele pode representar a assinatura à qual o recurso pertence.|

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


