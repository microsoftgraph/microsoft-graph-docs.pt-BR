---
title: tipo de recurso address
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7d168e4f53dbd182e4dbd93d0a5b6342daf3339d
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057323"
---
# <a name="postaladdress-resource-type"></a><span data-ttu-id="6a58c-103">tipo de recurso address</span><span class="sxs-lookup"><span data-stu-id="6a58c-103">postalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a58c-104">Representa o endereço da rua de um local.</span><span class="sxs-lookup"><span data-stu-id="6a58c-104">Represents the street address of a location.</span></span>


## <a name="properties"></a><span data-ttu-id="6a58c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a58c-105">Properties</span></span>
| <span data-ttu-id="6a58c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a58c-106">Property</span></span>     | <span data-ttu-id="6a58c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a58c-107">Type</span></span>   |<span data-ttu-id="6a58c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a58c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a58c-109">city</span><span class="sxs-lookup"><span data-stu-id="6a58c-109">city</span></span>|<span data-ttu-id="6a58c-110">String</span><span class="sxs-lookup"><span data-stu-id="6a58c-110">String</span></span>|<span data-ttu-id="6a58c-111">A cidade.</span><span class="sxs-lookup"><span data-stu-id="6a58c-111">The city.</span></span>|
|<span data-ttu-id="6a58c-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="6a58c-112">countryOrRegion</span></span>|<span data-ttu-id="6a58c-113">String</span><span class="sxs-lookup"><span data-stu-id="6a58c-113">String</span></span>|<span data-ttu-id="6a58c-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="6a58c-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="6a58c-116">isInferred</span><span class="sxs-lookup"><span data-stu-id="6a58c-116">isInferred</span></span>|<span data-ttu-id="6a58c-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a58c-117">Boolean</span></span>|<span data-ttu-id="6a58c-118">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="6a58c-118">For internal use only.</span></span>|
|<span data-ttu-id="6a58c-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="6a58c-119">postalCode</span></span>|<span data-ttu-id="6a58c-120">String</span><span class="sxs-lookup"><span data-stu-id="6a58c-120">String</span></span>|<span data-ttu-id="6a58c-121">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="6a58c-121">The postal code.</span></span>|
|<span data-ttu-id="6a58c-122">state</span><span class="sxs-lookup"><span data-stu-id="6a58c-122">state</span></span>|<span data-ttu-id="6a58c-123">String</span><span class="sxs-lookup"><span data-stu-id="6a58c-123">String</span></span>|<span data-ttu-id="6a58c-124">O estado.</span><span class="sxs-lookup"><span data-stu-id="6a58c-124">The state.</span></span>|
|<span data-ttu-id="6a58c-125">street</span><span class="sxs-lookup"><span data-stu-id="6a58c-125">street</span></span>|<span data-ttu-id="6a58c-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a58c-126">String</span></span>|<span data-ttu-id="6a58c-127">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="6a58c-127">The street.</span></span>|
|<span data-ttu-id="6a58c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a58c-128">type</span></span>|<span data-ttu-id="6a58c-129">addressType</span><span class="sxs-lookup"><span data-stu-id="6a58c-129">addressType</span></span>|<span data-ttu-id="6a58c-130">O tipo de endereço.</span><span class="sxs-lookup"><span data-stu-id="6a58c-130">The type of address.</span></span> <span data-ttu-id="6a58c-131">Os valores possíveis são: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="6a58c-131">The possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6a58c-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a58c-132">JSON representation</span></span>

<span data-ttu-id="6a58c-133">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6a58c-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.postalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "isInferred": "boolean",
  "postalCode": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "postaladdress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/postaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
