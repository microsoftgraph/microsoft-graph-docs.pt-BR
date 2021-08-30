---
author: swapnil1993
title: Tipo de recurso termColumn
description: O recurso termColumn indica que os valores da coluna contêm dados de taxonomia.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 38fa6fe4fdb7b08f93287305e43dddb4ec6d9331
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696484"
---
# <a name="termcolumn-resource-type"></a>Tipo de recurso termColumn

Namespace: microsoft.graph

Representa uma coluna de metadados gerenciados SharePoint.

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição|
|:--------------|:-------|:----------------------------------------------------|
| allowMultipleValues | Booliano | Especifica se a coluna permitirá mais de um valor.|
| parentTerm     | microsoft.graph.termStore.term | Especifica o termo GUID cujos filhos podem ser selecionados como o valor da coluna.  |
| showFullyQualifiedName | Booliano | Especifica se o caminho do termo inteiro será exibido ou somente o rótulo do termo.  |
| termSet      | microsoft.graph.termStore.set | Termset cujos filhos podem ser selecionados como o valor da coluna. |

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um **recurso termColumn.**
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "parentTerm": { "@type": "microsoft.graph.termStore.term" },
    "showFullyQualifiedName": false,
    "termSet": { "@type": "microsoft.graph.termStore.set" }
}
```

