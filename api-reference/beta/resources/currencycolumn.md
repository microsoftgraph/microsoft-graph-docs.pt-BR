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
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="89b4e-103">Tipo de recurso CurrencyColumn</span><span class="sxs-lookup"><span data-stu-id="89b4e-103">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89b4e-104">**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.</span><span class="sxs-lookup"><span data-stu-id="89b4e-104">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89b4e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89b4e-105">JSON representation</span></span>

<span data-ttu-id="89b4e-106">Aqui está uma representação JSON de um recurso **currencyColumn**.</span><span class="sxs-lookup"><span data-stu-id="89b4e-106">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="89b4e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89b4e-107">Properties</span></span>

| <span data-ttu-id="89b4e-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="89b4e-108">Property name</span></span> | <span data-ttu-id="89b4e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="89b4e-109">Type</span></span>   | <span data-ttu-id="89b4e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="89b4e-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="89b4e-111">**locale**</span><span class="sxs-lookup"><span data-stu-id="89b4e-111">**locale**</span></span>    | <span data-ttu-id="89b4e-112">string</span><span class="sxs-lookup"><span data-stu-id="89b4e-112">string</span></span> | <span data-ttu-id="89b4e-113">Especifica a localidade da qual o símbolo de moeda deverá ser inferido.</span><span class="sxs-lookup"><span data-stu-id="89b4e-113">Specifies the locale from which to infer the currency symbol.</span></span>

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
