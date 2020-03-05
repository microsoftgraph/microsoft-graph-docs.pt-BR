---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 53b1e18bd1e7b78e7afb479cac3c5f6cc7ecff88
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521873"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="af61a-103">Tipo de recurso physicalAddress</span><span class="sxs-lookup"><span data-stu-id="af61a-103">physicalAddress resource type</span></span>

<span data-ttu-id="af61a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="af61a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af61a-105">Representa o endereço físico de um recurso, como um contato ou evento.</span><span class="sxs-lookup"><span data-stu-id="af61a-105">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="af61a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af61a-106">Properties</span></span>
| <span data-ttu-id="af61a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af61a-107">Property</span></span>     | <span data-ttu-id="af61a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="af61a-108">Type</span></span>   |<span data-ttu-id="af61a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="af61a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af61a-110">city</span><span class="sxs-lookup"><span data-stu-id="af61a-110">city</span></span>|<span data-ttu-id="af61a-111">String</span><span class="sxs-lookup"><span data-stu-id="af61a-111">String</span></span>|<span data-ttu-id="af61a-112">A cidade.</span><span class="sxs-lookup"><span data-stu-id="af61a-112">The city.</span></span>|
|<span data-ttu-id="af61a-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="af61a-113">countryOrRegion</span></span>|<span data-ttu-id="af61a-114">String</span><span class="sxs-lookup"><span data-stu-id="af61a-114">String</span></span>|<span data-ttu-id="af61a-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="af61a-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="af61a-117">postalCode</span><span class="sxs-lookup"><span data-stu-id="af61a-117">postalCode</span></span>|<span data-ttu-id="af61a-118">String</span><span class="sxs-lookup"><span data-stu-id="af61a-118">String</span></span>|<span data-ttu-id="af61a-119">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="af61a-119">The postal code.</span></span>|
|<span data-ttu-id="af61a-120">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="af61a-120">postOfficeBox</span></span>|<span data-ttu-id="af61a-121">String</span><span class="sxs-lookup"><span data-stu-id="af61a-121">String</span></span>|<span data-ttu-id="af61a-122">O número da caixa postal.</span><span class="sxs-lookup"><span data-stu-id="af61a-122">The post office box number.</span></span>|
|<span data-ttu-id="af61a-123">state</span><span class="sxs-lookup"><span data-stu-id="af61a-123">state</span></span>|<span data-ttu-id="af61a-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af61a-124">String</span></span>|<span data-ttu-id="af61a-125">O estado.</span><span class="sxs-lookup"><span data-stu-id="af61a-125">The state.</span></span>|
|<span data-ttu-id="af61a-126">street</span><span class="sxs-lookup"><span data-stu-id="af61a-126">street</span></span>|<span data-ttu-id="af61a-127">String</span><span class="sxs-lookup"><span data-stu-id="af61a-127">String</span></span>|<span data-ttu-id="af61a-128">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="af61a-128">The street.</span></span>|
|<span data-ttu-id="af61a-129">type</span><span class="sxs-lookup"><span data-stu-id="af61a-129">type</span></span>|<span data-ttu-id="af61a-130">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="af61a-130">physicalAddressType</span></span>|<span data-ttu-id="af61a-131">O tipo de endereço.</span><span class="sxs-lookup"><span data-stu-id="af61a-131">The type of address.</span></span> <span data-ttu-id="af61a-132">Os valores possíveis são: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="af61a-132">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="af61a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af61a-133">JSON representation</span></span>

<span data-ttu-id="af61a-134">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="af61a-134">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "postOfficeBox": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
