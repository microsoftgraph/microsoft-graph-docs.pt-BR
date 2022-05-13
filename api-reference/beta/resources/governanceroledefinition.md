---
title: Tipo de recurso governanceRoleDefinition
description: Representa as definições de função. Para recursos do Azure, ele pode representar funções do RBAC do Azure, como Proprietário, Leitor, Colaborador etc.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 5cbb9cb86664407018237def427381610d898ff5
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398818"
---
# <a name="governanceroledefinition-resource-type"></a>Tipo de recurso governanceRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]


Representa as definições de função. Para recursos do Azure, ele pode representar funções do RBAC do Azure, como Proprietário, Leitor, Colaborador etc.


## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:--------|
|[Listar](../api/governanceroledefinition-list.md) | [coleção governanceRoleDefinition](../resources/governanceroledefinition.md) |Listar uma coleção de definições de função em um recurso.|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Ler propriedades e relações de uma entidade de definição de função especificada pela ID.|

Não `POST`, `PUT`, `PATCH`tem `DELETE` suporte no conjunto `roleDefinitions` de entidades por enquanto.

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| id          | Cadeia de caracteres | A ID da definição de função.                                        |
| resourceId  | Cadeia de caracteres | Obrigatório. A ID do recurso associado à definição de função. |
| externalId  | Cadeia de caracteres | A ID externa da definição de função.                               |
| displayName | Cadeia de caracteres | O nome de exibição da definição de função.                              |
| Templateid  | Cadeia de caracteres |                                                                       |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Somente leitura. O recurso associado para a definição de função.|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|A configuração de função associada para a definição de função.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
  "templateId":"String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


