---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: eb7bf1ee21a40517704f20176f5fbcf9ea2b276a
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30056984"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="a78d7-103">Tipo de recurso physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a78d7-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a78d7-104">Representa o endereço físico de um recurso, como um contato ou evento.</span><span class="sxs-lookup"><span data-stu-id="a78d7-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="a78d7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a78d7-105">Properties</span></span>
| <span data-ttu-id="a78d7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a78d7-106">Property</span></span>     | <span data-ttu-id="a78d7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a78d7-107">Type</span></span>   |<span data-ttu-id="a78d7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a78d7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a78d7-109">city</span><span class="sxs-lookup"><span data-stu-id="a78d7-109">city</span></span>|<span data-ttu-id="a78d7-110">String</span><span class="sxs-lookup"><span data-stu-id="a78d7-110">String</span></span>|<span data-ttu-id="a78d7-111">A cidade.</span><span class="sxs-lookup"><span data-stu-id="a78d7-111">The city.</span></span>|
|<span data-ttu-id="a78d7-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="a78d7-112">countryOrRegion</span></span>|<span data-ttu-id="a78d7-113">String</span><span class="sxs-lookup"><span data-stu-id="a78d7-113">String</span></span>|<span data-ttu-id="a78d7-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="a78d7-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="a78d7-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="a78d7-116">postalCode</span></span>|<span data-ttu-id="a78d7-117">String</span><span class="sxs-lookup"><span data-stu-id="a78d7-117">String</span></span>|<span data-ttu-id="a78d7-118">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="a78d7-118">The postal code.</span></span>|
|<span data-ttu-id="a78d7-119">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="a78d7-119">postOfficeBox</span></span>|<span data-ttu-id="a78d7-120">String</span><span class="sxs-lookup"><span data-stu-id="a78d7-120">String</span></span>|<span data-ttu-id="a78d7-121">O número da caixa postal.</span><span class="sxs-lookup"><span data-stu-id="a78d7-121">The post office box number.</span></span>|
|<span data-ttu-id="a78d7-122">estado</span><span class="sxs-lookup"><span data-stu-id="a78d7-122">state</span></span>|<span data-ttu-id="a78d7-123">String</span><span class="sxs-lookup"><span data-stu-id="a78d7-123">String</span></span>|<span data-ttu-id="a78d7-124">O estado.</span><span class="sxs-lookup"><span data-stu-id="a78d7-124">The state.</span></span>|
|<span data-ttu-id="a78d7-125">street</span><span class="sxs-lookup"><span data-stu-id="a78d7-125">street</span></span>|<span data-ttu-id="a78d7-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a78d7-126">String</span></span>|<span data-ttu-id="a78d7-127">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="a78d7-127">The street.</span></span>|
|<span data-ttu-id="a78d7-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a78d7-128">type</span></span>|<span data-ttu-id="a78d7-129">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="a78d7-129">physicalAddressType</span></span>|<span data-ttu-id="a78d7-130">O tipo de endereço.</span><span class="sxs-lookup"><span data-stu-id="a78d7-130">The type of address.</span></span> <span data-ttu-id="a78d7-131">Os valores possíveis são: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="a78d7-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a78d7-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a78d7-132">JSON representation</span></span>

<span data-ttu-id="a78d7-133">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a78d7-133">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/physicaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
