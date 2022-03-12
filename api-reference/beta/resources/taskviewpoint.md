---
title: Tipo de recurso taskViewpoint
description: Contém propriedades pessoais de uma tarefa"
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 36590611168f34335795f6200bfe06e09436c1c0
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451519"
---
# <a name="taskviewpoint-resource-type"></a>Tipo de recurso taskViewpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém propriedades pessoais de uma [tarefa](task.md). Ao compartilhar ou atribuir uma **tarefa**, essas propriedades não serão vistas por outros usuários.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data e a hora para que um alerta de lembrete da **tarefa** ocorra.|
|categories|Coleção de cadeias de caracteres|As categorias associadas à postagem. Cada categoria corresponde à propriedade **displayName** de uma [outlookCategory](../resources/outlookcategory.md) definida pelo usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.taskViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taskViewpoint",
  "reminderDatetime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "categories": ["string"]
}
```

