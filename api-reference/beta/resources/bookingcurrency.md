---
title: tipo de recurso bookingCurrency
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 6d04522b3a754e5a929fd48f8ea3c94f6ee5a6c3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453759"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="1f2d7-104">tipo de recurso bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="1f2d7-104">bookingCurrency resource type</span></span>

<span data-ttu-id="1f2d7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f2d7-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="1f2d7-106">Representa uma moeda monetária suportada por um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="1f2d7-106">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="1f2d7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1f2d7-107">Methods</span></span>

| <span data-ttu-id="1f2d7-108">Método</span><span class="sxs-lookup"><span data-stu-id="1f2d7-108">Method</span></span>           | <span data-ttu-id="1f2d7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1f2d7-109">Return Type</span></span>    |<span data-ttu-id="1f2d7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f2d7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f2d7-111">Listar bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="1f2d7-111">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="1f2d7-112">coleção [bookingCurrency](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="1f2d7-112">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="1f2d7-113">Obtenha uma lista de objetos **bookingCurrency** disponíveis para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1f2d7-113">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="1f2d7-114">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="1f2d7-114">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="1f2d7-115">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="1f2d7-115">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="1f2d7-116">Obter as propriedades de um objeto **bookingCurrency** .</span><span class="sxs-lookup"><span data-stu-id="1f2d7-116">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="1f2d7-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f2d7-117">Properties</span></span>
| <span data-ttu-id="1f2d7-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f2d7-118">Property</span></span>     | <span data-ttu-id="1f2d7-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f2d7-119">Type</span></span>   |<span data-ttu-id="1f2d7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f2d7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f2d7-121">id</span><span class="sxs-lookup"><span data-stu-id="1f2d7-121">id</span></span>|<span data-ttu-id="1f2d7-122">String</span><span class="sxs-lookup"><span data-stu-id="1f2d7-122">String</span></span>| <span data-ttu-id="1f2d7-123">Um código de moeda de 3 caracteres, com base na [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="1f2d7-123">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="1f2d7-124">Por exemplo, o código de moeda dos Dólar dos EUA é USD, e para o dólar australiano é AUD.</span><span class="sxs-lookup"><span data-stu-id="1f2d7-124">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="1f2d7-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f2d7-125">Read-only.</span></span>|
|<span data-ttu-id="1f2d7-126">formato</span><span class="sxs-lookup"><span data-stu-id="1f2d7-126">symbol</span></span>|<span data-ttu-id="1f2d7-127">String</span><span class="sxs-lookup"><span data-stu-id="1f2d7-127">String</span></span>| <span data-ttu-id="1f2d7-128">O símbolo da moeda.</span><span class="sxs-lookup"><span data-stu-id="1f2d7-128">The currency symbol.</span></span> <span data-ttu-id="1f2d7-129">Por exemplo, o símbolo de moeda dos dólar americano e para o dólar australiano é $.</span><span class="sxs-lookup"><span data-stu-id="1f2d7-129">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="1f2d7-130">Relações</span><span class="sxs-lookup"><span data-stu-id="1f2d7-130">Relationships</span></span>
<span data-ttu-id="1f2d7-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f2d7-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1f2d7-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f2d7-132">JSON representation</span></span>

<span data-ttu-id="1f2d7-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f2d7-133">The following is a JSON representation of the resource.</span></span>

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
