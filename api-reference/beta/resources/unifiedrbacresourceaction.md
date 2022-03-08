---
title: Tipo de recurso unifiedRbacResourceAction
description: Representa uma operação que uma entidade autorizada tem permissão para executar.
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4407c12d18576c6a6ad560588381bc7abd2b4855
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338085"
---
# <a name="unifiedrbacresourceaction-resource-type"></a>Tipo de recurso unifiedRbacResourceAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação que uma entidade autorizada tem permissão para executar.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRbacResourceActions](../api/unifiedrbacresourcenamespace-list-resourceactions.md)|[Coleção unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md)|Obter uma lista dos [objetos unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) e suas propriedades.|
|[Obter unifiedRbacResourceAction](../api/unifiedrbacresourceaction-get.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md)|Leia as propriedades e as relações de um [objeto unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionVerb|String|Método HTTP para a ação, como `DELETE`, `GET`, `PATCH`, , `POST`, `PUT`ou `null`. Oferece `$filter` suporte (`eq`) mas não para `null` valores. |
|description|String|Descrição da ação. Suporta `$filter` (`eq`). |
|id|String|Identificador exclusivo de uma ação dentro do namespace de recurso, como `microsoft.insights-programs-update-patch`. Não é possível incluir caractere de barra (`/`). Maiúsculas de minúsculas. Obrigatório. Suporta `$filter` (`eq`). |
|nome|String|Nome da ação dentro do namespace de recurso, como `microsoft.insights/programs/update`. Pode incluir caractere de barra (`/`). Maiúsculas de minúsculas. Obrigatório. Suporta `$filter` (`eq`). |
|resourceScopeId|String|Não implementado.|

## <a name="relationships"></a>Relações

Nenhum

<!-- The resourceScope relationship hasn't been implemented but is in the public schema. To unhide this and its related entities and methods once it's implemented.
|Relationship|Type|Description|
|:---|:---|:---|
|resourceScope| [unifiedRbacResourceScope](unifiedrbacresourcescope.md) |Not implemented.|
-->

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRbacResourceAction",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceAction",
  "id": "String (identifier)",
  "actionVerb": "String",
  "description": "String",
  "name": "String",
  "resourceScopeId": "String"
}
```
