---
title: tipo de recurso de privilegedRole
description: 'Representa uma função de administrador do Azure AD, tais como: **Administrador Global, administrador de faturamento, administrador de serviço, administrador do usuário, senha de administrador**, etc.'
localization_priority: Normal
ms.openlocfilehash: 75763e18731cb969623cc4df6360d50abc018b41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860855"
---
# <a name="privilegedrole-resource-type"></a>tipo de recurso de privilegedRole

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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

## <a name="relationships"></a>Relações
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
