---
title: tipo de recurso bookingCurrency
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: f4b5cc6a8fdb36c2e4543302ac32846a1b3c4388
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071791"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="ab7ef-104">tipo de recurso bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="ab7ef-104">bookingCurrency resource type</span></span>

<span data-ttu-id="ab7ef-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab7ef-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="ab7ef-106">Representa uma moeda monetária suportada por um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="ab7ef-106">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="ab7ef-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ab7ef-107">Methods</span></span>

| <span data-ttu-id="ab7ef-108">Método</span><span class="sxs-lookup"><span data-stu-id="ab7ef-108">Method</span></span>           | <span data-ttu-id="ab7ef-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ab7ef-109">Return Type</span></span>    |<span data-ttu-id="ab7ef-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab7ef-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab7ef-111">Listar bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="ab7ef-111">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="ab7ef-112">coleção [bookingCurrency](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="ab7ef-112">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="ab7ef-113">Obtenha uma lista de objetos **bookingCurrency** disponíveis para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ab7ef-113">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="ab7ef-114">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="ab7ef-114">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="ab7ef-115">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="ab7ef-115">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="ab7ef-116">Obter as propriedades de um objeto **bookingCurrency** .</span><span class="sxs-lookup"><span data-stu-id="ab7ef-116">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="ab7ef-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab7ef-117">Properties</span></span>
| <span data-ttu-id="ab7ef-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab7ef-118">Property</span></span>     | <span data-ttu-id="ab7ef-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab7ef-119">Type</span></span>   |<span data-ttu-id="ab7ef-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab7ef-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab7ef-121">id</span><span class="sxs-lookup"><span data-stu-id="ab7ef-121">id</span></span>|<span data-ttu-id="ab7ef-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab7ef-122">String</span></span>| <span data-ttu-id="ab7ef-123">Um código de moeda de 3 caracteres, com base na [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="ab7ef-123">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="ab7ef-124">Por exemplo, o código de moeda dos Dólar dos EUA é USD, e para o dólar australiano é AUD.</span><span class="sxs-lookup"><span data-stu-id="ab7ef-124">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="ab7ef-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab7ef-125">Read-only.</span></span>|
|<span data-ttu-id="ab7ef-126">formato</span><span class="sxs-lookup"><span data-stu-id="ab7ef-126">symbol</span></span>|<span data-ttu-id="ab7ef-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab7ef-127">String</span></span>| <span data-ttu-id="ab7ef-128">O símbolo da moeda.</span><span class="sxs-lookup"><span data-stu-id="ab7ef-128">The currency symbol.</span></span> <span data-ttu-id="ab7ef-129">Por exemplo, o símbolo de moeda dos dólar americano e para o dólar australiano é $.</span><span class="sxs-lookup"><span data-stu-id="ab7ef-129">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="ab7ef-130">Relações</span><span class="sxs-lookup"><span data-stu-id="ab7ef-130">Relationships</span></span>
<span data-ttu-id="ab7ef-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab7ef-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ab7ef-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab7ef-132">JSON representation</span></span>

<span data-ttu-id="ab7ef-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab7ef-133">The following is a JSON representation of the resource.</span></span>

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


