---
title: tipo de recurso bookingCurrency
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: f7b12f8ac48457ed0ea36c2fec2aa39be2ff7a01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013112"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="0cb85-104">tipo de recurso bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="0cb85-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="0cb85-105">Representa uma moeda monetária suportada por um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="0cb85-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="0cb85-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0cb85-106">Methods</span></span>

| <span data-ttu-id="0cb85-107">Método</span><span class="sxs-lookup"><span data-stu-id="0cb85-107">Method</span></span>           | <span data-ttu-id="0cb85-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0cb85-108">Return Type</span></span>    |<span data-ttu-id="0cb85-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cb85-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cb85-110">Listar bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="0cb85-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="0cb85-111">coleção [bookingCurrency](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="0cb85-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="0cb85-112">Obtenha uma lista de objetos **bookingCurrency** disponíveis para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0cb85-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="0cb85-113">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="0cb85-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="0cb85-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="0cb85-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="0cb85-115">Obter as propriedades de um objeto **bookingCurrency** .</span><span class="sxs-lookup"><span data-stu-id="0cb85-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="0cb85-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cb85-116">Properties</span></span>
| <span data-ttu-id="0cb85-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cb85-117">Property</span></span>     | <span data-ttu-id="0cb85-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cb85-118">Type</span></span>   |<span data-ttu-id="0cb85-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cb85-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cb85-120">id</span><span class="sxs-lookup"><span data-stu-id="0cb85-120">id</span></span>|<span data-ttu-id="0cb85-121">String</span><span class="sxs-lookup"><span data-stu-id="0cb85-121">String</span></span>| <span data-ttu-id="0cb85-122">Um código de moeda de 3 caracteres, com base na [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="0cb85-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="0cb85-123">Por exemplo, o código de moeda dos Dólar dos EUA é USD, e para o dólar australiano é AUD.</span><span class="sxs-lookup"><span data-stu-id="0cb85-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="0cb85-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0cb85-124">Read-only.</span></span>|
|<span data-ttu-id="0cb85-125">formato</span><span class="sxs-lookup"><span data-stu-id="0cb85-125">symbol</span></span>|<span data-ttu-id="0cb85-126">String</span><span class="sxs-lookup"><span data-stu-id="0cb85-126">String</span></span>| <span data-ttu-id="0cb85-127">O símbolo da moeda.</span><span class="sxs-lookup"><span data-stu-id="0cb85-127">The currency symbol.</span></span> <span data-ttu-id="0cb85-128">Por exemplo, o símbolo de moeda dos dólar americano e para o dólar australiano é $.</span><span class="sxs-lookup"><span data-stu-id="0cb85-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="0cb85-129">Relações</span><span class="sxs-lookup"><span data-stu-id="0cb85-129">Relationships</span></span>
<span data-ttu-id="0cb85-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0cb85-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0cb85-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cb85-131">JSON representation</span></span>

<span data-ttu-id="0cb85-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0cb85-132">The following is a JSON representation of the resource.</span></span>

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
