---
author: JeremyKelley
description: currencyColumn em um recurso columnDefinition indica que os valores da coluna representam moeda.
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 61a3c968ff48cd3bf59ec3611bc2e50a1a92a797
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973171"
---
# <a name="currencycolumn-resource-type"></a>Tipo de recurso CurrencyColumn

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
