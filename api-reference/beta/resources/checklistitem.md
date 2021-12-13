---
title: Tipo de recurso checklistItem
description: Representa uma coleção de itens de lista de verificação em uma tarefa
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 01cca362ac85b10cb4bf141908d2b5dac309c9cd
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424806"
---
# <a name="checklistitem-resource-type"></a>Tipo de recurso checklistItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de itens de lista de verificação em uma tarefa. **ChecklistItem** ajuda a dividir tarefas complexas em etapas menores e mais ativas.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar checklistItems](../api/basetask-list-checklistitems.md)|[Coleção checklistItem](../resources/checklistitem.md)|Obter uma lista dos [objetos checklistItem](../resources/checklistitem.md) e suas propriedades.|
|[Criar checklistItem](../api/basetask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Crie um novo [objeto checklistItem.](../resources/checklistitem.md)|
|[Obter checklistItem](../api/checklistitem-get.md)|[checklistItem](../resources/checklistitem.md)|Leia as propriedades e as relações de um [objeto checklistItem.](../resources/checklistitem.md)|
|[Atualizar checklistItem](../api/checklistitem-update.md)|[checklistItem](../resources/checklistitem.md)|Atualize as propriedades de um [objeto checklistItem.](../resources/checklistitem.md)|
|[Excluir checklistItem](../api/checklistitem-delete.md)|Nenhum|Exclui um [objeto checklistItem.](../resources/checklistitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|checkedDateTime|DateTimeOffset|A data e a hora em que **o checklistItem** foi concluído.|
|createdDateTime|DateTimeOffset|A data e a hora em que **o checklistItem** foi criado.|
|displayName|String|Campo que indica o título **de checklistItem**.|
|id|String|ID gerada do servidor para **checkListItem**|
|isChecked|Boolean|Estado indicando se o item foi verificado ou não.|

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

