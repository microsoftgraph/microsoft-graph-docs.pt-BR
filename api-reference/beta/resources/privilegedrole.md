---
title: Tipo de recurso privilegedRole
description: 'Representa uma função de administrador do Azure AD, como: **Administrador Global,** Administrador de Cobrança, Administrador de Serviço, Administrador de Usuário, Administrador de Senha etc.'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 5784a28ec18c0ed02540321d92ee2bab386dc760
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58452411"
---
# <a name="privilegedrole-resource-type"></a>Tipo de recurso privilegedRole

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma função de administrador do Azure AD, como: **Administrador Global,** Administrador de Cobrança, Administrador de Serviço, Administrador de Usuário, Administrador de Senha etc.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar objetos privilegedRole](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md) collection|Obter a coleção privilegedRole.|
|[Get privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |Ler propriedades e relações do objeto privilegedRole.|
|[Listar tarefas](../api/privilegedrole-list-assignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md) collection| Obter uma coleção de objetos de atribuição para essa função.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Ative a função atribuída.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Desative a função atribuída.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|string|O identificador exclusivo da função de administrador. É uma cadeia de caracteres GUID e tem o mesmo valor que a id do modelo de função do Azure AD para a função determinada. Somente leitura.|
|name|string|Nome da função.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignments|[privilegedRoleAssignment](privilegedroleassignment.md) collection| As atribuições dessa função. Somente leitura. Anulável.|
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


