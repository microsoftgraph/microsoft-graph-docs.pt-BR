---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: e4ee085882cadafc0102ee31e17841978cef7822
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836453"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="41a63-102">Tipo de recurso CurrencyColumn</span><span class="sxs-lookup"><span data-stu-id="41a63-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="41a63-103">**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.</span><span class="sxs-lookup"><span data-stu-id="41a63-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41a63-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41a63-104">JSON representation</span></span>

<span data-ttu-id="41a63-105">Aqui está uma representação JSON de um recurso **currencyColumn**.</span><span class="sxs-lookup"><span data-stu-id="41a63-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="41a63-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41a63-106">Properties</span></span>

| <span data-ttu-id="41a63-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="41a63-107">Property name</span></span> | <span data-ttu-id="41a63-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="41a63-108">Type</span></span>   | <span data-ttu-id="41a63-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="41a63-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="41a63-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="41a63-110">**locale**</span></span>    | <span data-ttu-id="41a63-111">string</span><span class="sxs-lookup"><span data-stu-id="41a63-111">string</span></span> | <span data-ttu-id="41a63-112">Especifica a localidade da qual o símbolo de moeda deverá ser inferido.</span><span class="sxs-lookup"><span data-stu-id="41a63-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
