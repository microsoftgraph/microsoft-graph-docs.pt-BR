---
author: JeremyKelley
description: currencyColumn em um recurso columnDefinition indica que os valores da coluna representam moeda.
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 75ef7125c55674b2feb6e617a40313b5bca242bc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507328"
---
# <a name="currencycolumn-resource-type"></a>Tipo de recurso CurrencyColumn

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **currencyColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| **locale**    | string | Especifica a localidade da qual o símbolo de moeda deverá ser inferido.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": []
}
-->
