---
title: Tipo de recurso privilegedRole
description: 'Representa uma função de administrador do Azure AD, como: Administrador Global, Administrador de Cobrança, Administrador de Serviço, Administrador de Usuário e Administrador de Senha.'
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 756ffd580a2f44fad1631bbfd153d1320f1aef05
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687673"
---
# <a name="privilegedrole-resource-type-deprecated"></a>Tipo de recurso privilegedRole (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1AADRoles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

Representa uma função de administrador interna do [Azure AD](/azure/active-directory/roles/permissions-reference), por exemplo, **Administrador Global,** Administrador de Cobrança, Administrador de Serviço, Administrador de Usuário e **Administrador de Senha.**


## <a name="methods"></a>Methods

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
|id|cadeia de caracteres|O identificador exclusivo da função de administrador. É uma cadeia de caracteres GUID e tem o mesmo valor que a id do modelo de função do Azure AD para a função determinada. Somente leitura.|
|name|string|Nome da função.|

## <a name="relationships"></a>Relações
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


