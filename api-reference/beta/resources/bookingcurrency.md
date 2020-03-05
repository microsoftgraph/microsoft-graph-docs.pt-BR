---
title: tipo de recurso bookingCurrency
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c1d56dde0c239245f6724040229df7d417a79613
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508000"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="d014a-104">tipo de recurso bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="d014a-104">bookingCurrency resource type</span></span>

<span data-ttu-id="d014a-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d014a-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="d014a-106">Representa uma moeda monetária suportada por um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="d014a-106">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="d014a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d014a-107">Methods</span></span>

| <span data-ttu-id="d014a-108">Método</span><span class="sxs-lookup"><span data-stu-id="d014a-108">Method</span></span>           | <span data-ttu-id="d014a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d014a-109">Return Type</span></span>    |<span data-ttu-id="d014a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d014a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d014a-111">Listar bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="d014a-111">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="d014a-112">coleção [bookingCurrency](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="d014a-112">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="d014a-113">Obtenha uma lista de objetos **bookingCurrency** disponíveis para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d014a-113">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="d014a-114">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="d014a-114">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="d014a-115">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="d014a-115">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="d014a-116">Obter as propriedades de um objeto **bookingCurrency** .</span><span class="sxs-lookup"><span data-stu-id="d014a-116">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="d014a-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d014a-117">Properties</span></span>
| <span data-ttu-id="d014a-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d014a-118">Property</span></span>     | <span data-ttu-id="d014a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d014a-119">Type</span></span>   |<span data-ttu-id="d014a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d014a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d014a-121">id</span><span class="sxs-lookup"><span data-stu-id="d014a-121">id</span></span>|<span data-ttu-id="d014a-122">String</span><span class="sxs-lookup"><span data-stu-id="d014a-122">String</span></span>| <span data-ttu-id="d014a-123">Um código de moeda de 3 caracteres, com base na [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="d014a-123">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="d014a-124">Por exemplo, o código de moeda dos Dólar dos EUA é USD, e para o dólar australiano é AUD.</span><span class="sxs-lookup"><span data-stu-id="d014a-124">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="d014a-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d014a-125">Read-only.</span></span>|
|<span data-ttu-id="d014a-126">formato</span><span class="sxs-lookup"><span data-stu-id="d014a-126">symbol</span></span>|<span data-ttu-id="d014a-127">String</span><span class="sxs-lookup"><span data-stu-id="d014a-127">String</span></span>| <span data-ttu-id="d014a-128">O símbolo da moeda.</span><span class="sxs-lookup"><span data-stu-id="d014a-128">The currency symbol.</span></span> <span data-ttu-id="d014a-129">Por exemplo, o símbolo de moeda dos dólar americano e para o dólar australiano é $.</span><span class="sxs-lookup"><span data-stu-id="d014a-129">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="d014a-130">Relações</span><span class="sxs-lookup"><span data-stu-id="d014a-130">Relationships</span></span>
<span data-ttu-id="d014a-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d014a-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d014a-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d014a-132">JSON representation</span></span>

<span data-ttu-id="d014a-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d014a-133">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
