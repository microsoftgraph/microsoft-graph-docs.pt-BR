---
title: tipo de recurso de bookingCurrency
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9d4feac66e72c756173113101a88bf8bbe35563a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518195"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="97886-104">tipo de recurso de bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="97886-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="97886-105">Representa uma moeda monetária compatíveis com uma [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="97886-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="97886-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="97886-106">Methods</span></span>

| <span data-ttu-id="97886-107">Método</span><span class="sxs-lookup"><span data-stu-id="97886-107">Method</span></span>           | <span data-ttu-id="97886-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="97886-108">Return Type</span></span>    |<span data-ttu-id="97886-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="97886-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97886-110">Lista bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="97886-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="97886-111">coleção [bookingCurrency](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="97886-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="97886-112">Obtenha uma lista de objetos de **bookingCurrency** disponíveis para uma empresa Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="97886-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="97886-113">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="97886-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="97886-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="97886-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="97886-115">Obtenha as propriedades de um objeto **bookingCurrency** .</span><span class="sxs-lookup"><span data-stu-id="97886-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="97886-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97886-116">Properties</span></span>
| <span data-ttu-id="97886-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97886-117">Property</span></span>     | <span data-ttu-id="97886-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="97886-118">Type</span></span>   |<span data-ttu-id="97886-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="97886-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97886-120">id</span><span class="sxs-lookup"><span data-stu-id="97886-120">id</span></span>|<span data-ttu-id="97886-121">String</span><span class="sxs-lookup"><span data-stu-id="97886-121">String</span></span>| <span data-ttu-id="97886-122">Um código de moeda de 3 caracteres, com base em [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="97886-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="97886-123">Por exemplo, o código de moeda para o dólar americano é USD e para o Dólar australiano é AUD.</span><span class="sxs-lookup"><span data-stu-id="97886-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="97886-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97886-124">Read-only.</span></span>|
|<span data-ttu-id="97886-125">Symbol</span><span class="sxs-lookup"><span data-stu-id="97886-125">symbol</span></span>|<span data-ttu-id="97886-126">String</span><span class="sxs-lookup"><span data-stu-id="97886-126">String</span></span>| <span data-ttu-id="97886-127">O símbolo da moeda.</span><span class="sxs-lookup"><span data-stu-id="97886-127">The currency symbol.</span></span> <span data-ttu-id="97886-128">Por exemplo, o símbolo de moeda para o dólar americano e para o Dólar australiano é $.</span><span class="sxs-lookup"><span data-stu-id="97886-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="97886-129">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="97886-129">Relationships</span></span>
<span data-ttu-id="97886-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97886-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="97886-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97886-131">JSON representation</span></span>

<span data-ttu-id="97886-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97886-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcurrency.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
