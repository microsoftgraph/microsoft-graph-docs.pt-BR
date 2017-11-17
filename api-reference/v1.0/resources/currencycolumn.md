---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 4f3ae97e5abfb84ad523caf74fa70b1f1ec0322a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="50736-102">Tipo de recurso CurrencyColumn</span><span class="sxs-lookup"><span data-stu-id="50736-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="50736-103">**currencyColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna representam moeda.</span><span class="sxs-lookup"><span data-stu-id="50736-103">The **currencyColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50736-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50736-104">JSON representation</span></span>

<span data-ttu-id="50736-105">Aqui está uma representação JSON de um recurso **currencyColumn**.</span><span class="sxs-lookup"><span data-stu-id="50736-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="50736-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50736-106">Properties</span></span>

| <span data-ttu-id="50736-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="50736-107">Property name</span></span> | <span data-ttu-id="50736-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="50736-108">Type</span></span>   | <span data-ttu-id="50736-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="50736-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="50736-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="50736-110">**locale**</span></span>    | <span data-ttu-id="50736-111">string</span><span class="sxs-lookup"><span data-stu-id="50736-111">string</span></span> | <span data-ttu-id="50736-112">Especifica a localidade da qual o símbolo de moeda deverá ser inferido.</span><span class="sxs-lookup"><span data-stu-id="50736-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
