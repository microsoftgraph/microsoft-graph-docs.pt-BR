---
title: Tipo de recurso governanceRoleDefinition
description: Representa as definições de função. Para recursos do Azure, ele pode representar funções do Azure RBAC, como Proprietário, Leitor, Colaborador, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 4f0144f4d26c8440b4e2bdc0965e88310a4f9145
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453720"
---
# <a name="governanceroledefinition-resource-type"></a>Tipo de recurso governanceRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Representa as definições de função. Para recursos do Azure, ele pode representar funções do Azure RBAC, como Proprietário, Leitor, Colaborador, etc.


## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:--------|
|[List](../api/governanceroledefinition-list.md) | [Coleção governanceRoleDefinition](../resources/governanceroledefinition.md) |Listar uma coleção de definições de função em um recurso.|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Ler propriedades e relações de uma entidade de definição de função especificada pela id.|

Não `POST` , , é suportado no conjunto de `PUT` `PATCH` `DELETE` `roleDefinitions` entidades por enquanto.

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| id          | Cadeia de caracteres | A id da definição de função.                                        |
| resourceId  | Cadeia de caracteres | Obrigatório. A id do recurso associado à definição de função. |
| externalId  | Cadeia de caracteres | A id externa da definição de função.                               |
| displayName | Cadeia de caracteres | O nome de exibição da definição de função.                              |
| templateId  | Cadeia de caracteres |                                                                       |

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Apenas leitura. O recurso associado para a definição de função.|
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


