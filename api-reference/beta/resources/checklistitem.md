---
title: Tipo de recurso checklistItem
description: Representa uma coleção de itens de lista de verificação em uma tarefa
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 86ec25ee83ae6cd1f30bf8a84b6177f870d39586
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451128"
---
# <a name="checklistitem-resource-type"></a>Tipo de recurso checklistItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma subtarefa em uma [baseTask maior](./baseTask.md). **ChecklistItem** permite separar uma tarefa complexa em tarefas mais ativas e menores. 

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar checklistItems](../api/basetask-list-checklistitems.md)|[Coleção checklistItem](../resources/checklistitem.md)|Obter uma lista dos [objetos checklistItem](../resources/checklistitem.md) e suas propriedades.|
|[Criar checklistItem](../api/basetask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Crie um novo [objeto checklistItem](../resources/checklistitem.md) .|
|[Obter checklistItem](../api/checklistitem-get.md)|[checklistItem](../resources/checklistitem.md)|Leia as propriedades e as relações de um [objeto checklistItem](../resources/checklistitem.md) .|
|[Atualizar checklistItem](../api/checklistitem-update.md)|[checklistItem](../resources/checklistitem.md)|Atualize as propriedades de um [objeto checklistItem](../resources/checklistitem.md) .|
|[Excluir checklistItem](../api/checklistitem-delete.md)|Nenhum|Exclui um [objeto checklistItem](../resources/checklistitem.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|checkedDateTime|DateTimeOffset|A data e a hora em que **o checklistItem** foi concluído.|
|createdDateTime|DateTimeOffset|A data e a hora em que **o checklistItem** foi criado.|
|displayName|Cadeia de caracteres|Campo que indica o título **de checklistItem**.|
|id|Cadeia de caracteres|ID gerada do servidor para **checkListItem**|
|isChecked|Booliano|Estado indicando se o item foi verificado ou não.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.checklistItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.checklistItem",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "checkedDateTime": "String (timestamp)",
  "isChecked": "Boolean",
  "id": "String (identifier)"
}
```

