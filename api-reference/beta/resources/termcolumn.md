---
author: swapnil1993
title: Tipo de recurso termColumn
description: O recurso termColumn indica que os valores da coluna contêm dados de taxonomia.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6d29ec570d7f3fad798fb1e2ba213b5a998643dc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445923"
---
# <a name="termcolumn-resource-type"></a>Tipo de recurso termColumn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Indica que os valores da coluna contêm dados de taxonomia.

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| allowMultipleValues | Booliano | Especifica se a coluna permitirá mais de um valor   
| parentTerm     | microsoft.graph.termStore.term | Especifica o guid do termo cujos filhos podem ser selecionados como o valor da coluna.  
| showFullyQualifiedName | Booliano | Especifica se o caminho do termo inteiro será exibido ou somente o rótulo do termo.  
| termSet      | microsoft.graph.termStore.set | Termset cujos filhos podem ser selecionados como o valor da coluna. 

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

