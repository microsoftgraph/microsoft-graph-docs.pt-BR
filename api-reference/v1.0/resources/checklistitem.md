---
title: Tipo de recurso checklistItem
description: Representa uma coleção de itens da lista de verificação em uma tarefa
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0c60add74b11b245c1fdf732ae1458fd2ed07bf0
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821294"
---
# <a name="checklistitem-resource-type"></a>Tipo de recurso checklistItem

Namespace: microsoft.graph

Representa uma subtarefa em um [todoTask maior](./todotask.md). **ChecklistItem** permite dividir uma tarefa complexa em tarefas mais acionáveis e menores. 

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar checklistItems](../api/todotask-list-checklistitems.md)|[coleção checklistItem](../resources/checklistitem.md)|Obtenha uma lista dos objetos [checklistItem](../resources/checklistitem.md) e suas propriedades.|
|[Criar checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Crie um novo [objeto checklistItem](../resources/checklistitem.md) .|
|[Obter checklistItem](../api/checklistitem-get.md)|[checklistItem](../resources/checklistitem.md)|Leia as propriedades e as relações de um [objeto checklistItem](../resources/checklistitem.md) .|
|[Atualizar checklistItem](../api/checklistitem-update.md)|[checklistItem](../resources/checklistitem.md)|Atualize as propriedades de um [objeto checklistItem](../resources/checklistitem.md) .|
|[Excluir checklistItem](../api/checklistitem-delete.md)|Nenhum|Exclui um [objeto checklistItem](../resources/checklistitem.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|checkedDateTime|DateTimeOffset|A data e a hora em que **o checklistItem** foi concluído.|
|createdDateTime|DateTimeOffset|A data e a hora em que **o checklistItem** foi criado.|
|displayName|Cadeia de caracteres|Campo que indica o título **de checklistItem**.|
|id|Cadeia de caracteres|ID gerada pelo servidor para **checkListItem**|
|Ischecked|Booliano|Estado que indica se o item foi verificado ou não.|

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

