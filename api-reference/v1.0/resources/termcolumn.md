---
author: swapnil1993
title: Tipo de recurso termColumn
description: O recurso termColumn indica que os valores da coluna contêm dados de taxonomia.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: cc5cb17f47425efb2732f5258cbdb1ac9bfff916
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757595"
---
# <a name="termcolumn-resource-type"></a>Tipo de recurso termColumn

Namespace: microsoft.graph

Representa uma coluna de metadados gerenciados SharePoint.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição|
|:--------------|:-------|:----------------------------------------------------|
| allowMultipleValues | Boolean | Especifica se a coluna permitirá mais de um valor.|
| showFullyQualifiedName | Booliano | Especifica se o caminho do termo inteiro será exibido ou somente o rótulo do termo.  |

## <a name="relationships"></a>Relações

| Relação   | Tipo                      | Descrição
|:----------------|:--------------------------|:-------------------------------
| parentTerm     | microsoft.graph.termStore.term | Especifica o termo pai para o qual os termos filho podem ser selecionados como o valor da coluna.
| termSet      | microsoft.graph.termStore.set | Termset cujos filhos podem ser selecionados como o valor da coluna. 

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um **recurso termColumn** .
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "showFullyQualifiedName": false,
}
```

