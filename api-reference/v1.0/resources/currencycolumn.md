---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 796bd9fc7bf379ea38dc2d2f602411740caf4b86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007209"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="5fada-102">Tipo de recurso CurrencyColumn</span><span class="sxs-lookup"><span data-stu-id="5fada-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="5fada-103">**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.</span><span class="sxs-lookup"><span data-stu-id="5fada-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fada-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fada-104">JSON representation</span></span>

<span data-ttu-id="5fada-105">Aqui está uma representação JSON de um recurso **currencyColumn**.</span><span class="sxs-lookup"><span data-stu-id="5fada-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="5fada-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fada-106">Properties</span></span>

| <span data-ttu-id="5fada-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5fada-107">Property name</span></span> | <span data-ttu-id="5fada-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fada-108">Type</span></span>   | <span data-ttu-id="5fada-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fada-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5fada-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="5fada-110">**locale**</span></span>    | <span data-ttu-id="5fada-111">string</span><span class="sxs-lookup"><span data-stu-id="5fada-111">string</span></span> | <span data-ttu-id="5fada-112">Especifica a localidade da qual o símbolo de moeda deverá ser inferido.</span><span class="sxs-lookup"><span data-stu-id="5fada-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
