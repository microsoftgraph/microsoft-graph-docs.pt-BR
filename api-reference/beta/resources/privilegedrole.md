---
title: tipo de recurso privilegedRole
description: Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 3d0b24022696fbb0df861ce0c2a78e0c9bbbd6e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070517"
---
# <a name="privilegedrole-resource-type"></a>tipo de recurso privilegedRole

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar objetos privilegedRole](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md) collection|Obtenha a coleção de privilegedRole.|
|[Get privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |Leia as propriedades e os relacionamentos do objeto privilegedRole.|
|[Listar tarefas](../api/privilegedrole-list-assignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md) collection| Obtenha uma coleção de objetos Assignment para essa função.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Ative a função atribuída.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Desative a função atribuída.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres|O identificador exclusivo para a função de administrador. É uma cadeia de caracteres GUID e tem o mesmo valor que a ID de modelo de função do Azure AD para a função determinada. Somente leitura.|
|name|string|Nome da função.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignments|[privilegedRoleAssignment](privilegedroleassignment.md) collection| As atribuições para essa função. Somente leitura. Anulável.|
|settings|[privilegedRoleSettings](privilegedrolesettings.md)| As configurações dessa função. Somente leitura. Anulável.|
|summary|[privilegedRoleSummary](privilegedrolesummary.md)| As informações resumidas para essa função. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


