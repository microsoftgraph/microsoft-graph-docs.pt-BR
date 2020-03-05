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
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="eeb29-103">Tipo de recurso CurrencyColumn</span><span class="sxs-lookup"><span data-stu-id="eeb29-103">CurrencyColumn resource type</span></span>

<span data-ttu-id="eeb29-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eeb29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeb29-105">**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.</span><span class="sxs-lookup"><span data-stu-id="eeb29-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eeb29-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eeb29-106">JSON representation</span></span>

<span data-ttu-id="eeb29-107">Aqui está uma representação JSON de um recurso **currencyColumn**.</span><span class="sxs-lookup"><span data-stu-id="eeb29-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="eeb29-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eeb29-108">Properties</span></span>

| <span data-ttu-id="eeb29-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="eeb29-109">Property name</span></span> | <span data-ttu-id="eeb29-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeb29-110">Type</span></span>   | <span data-ttu-id="eeb29-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb29-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="eeb29-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="eeb29-112">**locale**</span></span>    | <span data-ttu-id="eeb29-113">string</span><span class="sxs-lookup"><span data-stu-id="eeb29-113">string</span></span> | <span data-ttu-id="eeb29-114">Especifica a localidade da qual o símbolo de moeda deverá ser inferido.</span><span class="sxs-lookup"><span data-stu-id="eeb29-114">Specifies the locale from which to infer the currency symbol.</span></span>

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
