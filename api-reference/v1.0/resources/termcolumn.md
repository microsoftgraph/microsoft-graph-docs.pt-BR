---
author: swapnil1993
title: Tipo de recurso termColumn
description: O recurso termColumn indica que os valores da coluna contêm dados de taxonomia.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d89d389b78c4c8dc1a370722a5b40c7cff794d3d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128036"
---
# <a name="termcolumn-resource-type"></a>Tipo de recurso termColumn

Namespace: microsoft.graph

Representa uma coluna de metadados gerenciados SharePoint.

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição|
|:--------------|:-------|:----------------------------------------------------|
| allowMultipleValues | Boolean | Especifica se a coluna permitirá mais de um valor.|
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

