---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d6081f21069cef6014c8a028898f11ea9a3f4f3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344967"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="b655e-103">Tipo de recurso physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b655e-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b655e-104">Representa o endereço físico de um recurso, como um contato ou evento.</span><span class="sxs-lookup"><span data-stu-id="b655e-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="b655e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b655e-105">Properties</span></span>
| <span data-ttu-id="b655e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b655e-106">Property</span></span>     | <span data-ttu-id="b655e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b655e-107">Type</span></span>   |<span data-ttu-id="b655e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b655e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b655e-109">city</span><span class="sxs-lookup"><span data-stu-id="b655e-109">city</span></span>|<span data-ttu-id="b655e-110">String</span><span class="sxs-lookup"><span data-stu-id="b655e-110">String</span></span>|<span data-ttu-id="b655e-111">A cidade.</span><span class="sxs-lookup"><span data-stu-id="b655e-111">The city.</span></span>|
|<span data-ttu-id="b655e-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b655e-112">countryOrRegion</span></span>|<span data-ttu-id="b655e-113">String</span><span class="sxs-lookup"><span data-stu-id="b655e-113">String</span></span>|<span data-ttu-id="b655e-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="b655e-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="b655e-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="b655e-116">postalCode</span></span>|<span data-ttu-id="b655e-117">String</span><span class="sxs-lookup"><span data-stu-id="b655e-117">String</span></span>|<span data-ttu-id="b655e-118">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="b655e-118">The postal code.</span></span>|
|<span data-ttu-id="b655e-119">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="b655e-119">postOfficeBox</span></span>|<span data-ttu-id="b655e-120">String</span><span class="sxs-lookup"><span data-stu-id="b655e-120">String</span></span>|<span data-ttu-id="b655e-121">O número da caixa postal.</span><span class="sxs-lookup"><span data-stu-id="b655e-121">The post office box number.</span></span>|
|<span data-ttu-id="b655e-122">state</span><span class="sxs-lookup"><span data-stu-id="b655e-122">state</span></span>|<span data-ttu-id="b655e-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b655e-123">String</span></span>|<span data-ttu-id="b655e-124">O estado.</span><span class="sxs-lookup"><span data-stu-id="b655e-124">The state.</span></span>|
|<span data-ttu-id="b655e-125">street</span><span class="sxs-lookup"><span data-stu-id="b655e-125">street</span></span>|<span data-ttu-id="b655e-126">String</span><span class="sxs-lookup"><span data-stu-id="b655e-126">String</span></span>|<span data-ttu-id="b655e-127">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="b655e-127">The street.</span></span>|
|<span data-ttu-id="b655e-128">type</span><span class="sxs-lookup"><span data-stu-id="b655e-128">type</span></span>|<span data-ttu-id="b655e-129">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="b655e-129">physicalAddressType</span></span>|<span data-ttu-id="b655e-130">O tipo de endereço.</span><span class="sxs-lookup"><span data-stu-id="b655e-130">The type of address.</span></span> <span data-ttu-id="b655e-131">Os valores possíveis são: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="b655e-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b655e-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b655e-132">JSON representation</span></span>

<span data-ttu-id="b655e-133">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b655e-133">Here is a JSON representation of the resource</span></span>

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
