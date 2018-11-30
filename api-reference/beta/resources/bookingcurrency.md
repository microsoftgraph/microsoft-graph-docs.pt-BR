---
title: tipo de recurso de bookingCurrency
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: a68b88160e42217f3605c4a4bb30f692e8dafc06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034591"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="d76ab-104">tipo de recurso de bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="d76ab-104">bookingCurrency resource type</span></span>

 > <span data-ttu-id="d76ab-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d76ab-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d76ab-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d76ab-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="d76ab-107">Representa uma moeda monetária compatíveis com uma [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="d76ab-107">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="d76ab-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d76ab-108">Methods</span></span>

| <span data-ttu-id="d76ab-109">Método</span><span class="sxs-lookup"><span data-stu-id="d76ab-109">Method</span></span>           | <span data-ttu-id="d76ab-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d76ab-110">Return Type</span></span>    |<span data-ttu-id="d76ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d76ab-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d76ab-112">Lista bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="d76ab-112">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="d76ab-113">coleção [bookingCurrency](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="d76ab-113">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="d76ab-114">Obtenha uma lista de objetos de **bookingCurrency** disponíveis para uma empresa Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="d76ab-114">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="d76ab-115">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="d76ab-115">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="d76ab-116">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="d76ab-116">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="d76ab-117">Obtenha as propriedades de um objeto **bookingCurrency** .</span><span class="sxs-lookup"><span data-stu-id="d76ab-117">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="d76ab-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d76ab-118">Properties</span></span>
| <span data-ttu-id="d76ab-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d76ab-119">Property</span></span>     | <span data-ttu-id="d76ab-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d76ab-120">Type</span></span>   |<span data-ttu-id="d76ab-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d76ab-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d76ab-122">id</span><span class="sxs-lookup"><span data-stu-id="d76ab-122">id</span></span>|<span data-ttu-id="d76ab-123">String</span><span class="sxs-lookup"><span data-stu-id="d76ab-123">String</span></span>| <span data-ttu-id="d76ab-124">Um código de moeda de 3 caracteres, com base em [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="d76ab-124">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="d76ab-125">Por exemplo, o código de moeda para o dólar americano é USD e para o Dólar australiano é AUD.</span><span class="sxs-lookup"><span data-stu-id="d76ab-125">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="d76ab-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d76ab-126">Read-only.</span></span>|
|<span data-ttu-id="d76ab-127">símbolo</span><span class="sxs-lookup"><span data-stu-id="d76ab-127">symbol</span></span>|<span data-ttu-id="d76ab-128">String</span><span class="sxs-lookup"><span data-stu-id="d76ab-128">String</span></span>| <span data-ttu-id="d76ab-129">O símbolo da moeda.</span><span class="sxs-lookup"><span data-stu-id="d76ab-129">The currency symbol.</span></span> <span data-ttu-id="d76ab-130">Por exemplo, o símbolo de moeda para o dólar americano e para o Dólar australiano é $.</span><span class="sxs-lookup"><span data-stu-id="d76ab-130">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="d76ab-131">Relações</span><span class="sxs-lookup"><span data-stu-id="d76ab-131">Relationships</span></span>
<span data-ttu-id="d76ab-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d76ab-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d76ab-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d76ab-133">JSON representation</span></span>

<span data-ttu-id="d76ab-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d76ab-134">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->