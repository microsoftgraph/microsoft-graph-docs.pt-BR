---
title: Tipo de recurso governanceResource
description: Representa recursos que podem ser gerenciados pelo PIM (Privileged Identity Management). Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso, como uma máquina virtual, um banco de dados SQL, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e0cf42593a35103996217d1ce18bd9938b48a185
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443108"
---
# <a name="governanceresource-resource-type"></a>Tipo de recurso governanceResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa recursos que podem ser gerenciados pelo PIM (Privileged Identity Management). Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso, como uma máquina virtual, um banco de dados SQL, etc.


## <a name="methods"></a>Methods

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [Coleção governanceResource](../resources/governanceresource.md)|Listar uma coleção de recursos aos que o solicitante tem acesso.|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Ler propriedades e relações de uma entidade de recurso especificada por id.|
|[Registrar](../api/governanceresource-register.md) | |Registre uma assinatura ou grupo de gerenciamento não gerenciada do Azure no serviço PIM. |

Não `POST` , , são `PUT` `PATCH` `DELETE` suportados no conjunto de `roleDefinitions` entidades por enquanto.

## <a name="properties"></a>Propriedades
| Propriedade          |Tipo         |Descrição|
|:------------------|:----------|:----------|
|id                 |String     |A id do recurso. Está no formato GUID.|
|externalId           |Cadeia de caracteres   |A id externa do recurso, representando sua id original no sistema externo. Por exemplo, a ID externa de um recurso de assinatura pode ser "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac". |
|type               |String     |Obrigatório. Tipo de recurso. Por exemplo, para recursos do Azure, o tipo pode ser "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.|
|displayName        |String     |O nome de exibição do recurso.|
|status             |String     |O status de um determinado recurso. Por exemplo, ele pode representar se o recurso está bloqueado ou não (valores: `Active` / `Locked` ). Observação: essa propriedade pode ser estendida no futuro para dar suporte a mais cenários.|
|registeredDateTime|DateTimeOffset      |Representa a data em que o recurso é registrado no PIM.|
|registeredRoot|String      |O externalId do escopo raiz do recurso que está registrado no PIM. O escopo raiz pode ser o pai, o vôrent ou recursos ancestrais superiores.|
|roleAssignmentCount|Int32      |Opcional. O número de atribuições de função para o recurso determinado. Para obter a propriedade, use explictly `$select=roleAssignmentCount` na consulta.|
|roleDefinitionCount|Int32      |Opcional. O número de definições de função para o determinado recurso. Para obter a propriedade, use explictly `$select=roleDefinitionCount` na consulta.|
|permissões|[governancePermission](../resources/governancepermission.md)      |Opcional. Ele representa o status do acesso do solicitante ao recurso. Para obter a propriedade, use explictly `$select=permissions` na consulta.|

## <a name="relationships"></a>Relações
| Relação   | Tipo                                         |Descrição|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[Coleção governanceRoleAssignment](../resources/governanceroleassignment.md)|A coleção de atribuições de função para o recurso.|
|roleDefinitions |[Coleção governanceRoleDefinition](../resources/governanceroledefinition.md)|A coleção de definições de função para o recurso.|
|roleAssignmentRequests |[Coleção governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|A coleção de solicitações de atribuição de função para o recurso.|
|roleSettings |[Coleção governanceRoleSetting](../resources/governancerolesetting.md)|A coleção de configurações de função do recurso.|
|primário          |[governanceResource](../resources/governanceresource.md)           |Somente leitura. O recurso pai. para `pimforazurerbac` cenário, ele pode representar a assinatura à que o recurso pertence.|

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


