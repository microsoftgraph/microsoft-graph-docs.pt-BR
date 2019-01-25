---
title: tipo de recurso de privilegedRole
description: 'Representa uma função de administrador do Azure AD, tais como: **Administrador Global, administrador de faturamento, administrador de serviço, administrador do usuário, senha de administrador**, etc.'
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513743"
---
# <a name="privilegedrole-resource-type"></a>tipo de recurso de privilegedRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma função de administrador do Azure AD, tais como: **Administrador Global, administrador de faturamento, administrador de serviço, administrador do usuário, senha de administrador**, etc.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Objetos de privilegedRole List](../api/privilegedrole-list.md) | coleção [privilegedRole](privilegedrole.md)|Obtenha a coleção de privilegedRole.|
|[Obter privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |Leia as propriedades e os relacionamentos do objeto privilegedRole.|
|[Lista de atribuições](../api/privilegedrole-list-assignments.md) |coleção [privilegedRoleAssignment](privilegedroleassignment.md)| Obtenha uma coleção de objetos de atribuição para essa função.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Ative a função atribuída.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Desative a função atribuída.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|string|O identificador exclusivo para a função de administrador. É uma cadeia de caracteres GUID e tem o mesmo valor que a identificação do modelo de função do Azure AD para uma determinada função. Somente leitura.|
|name|string|Nome da função.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignments|coleção [privilegedRoleAssignment](privilegedroleassignment.md)| As atribuições para essa função. Somente leitura. Anulável.|
|configurações|[privilegedRoleSettings](privilegedrolesettings.md)| As configurações para essa função. Somente leitura. Anulável.|
|Resumo|[privilegedRoleSummary](privilegedrolesummary.md)| As informações de resumo para essa função. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
