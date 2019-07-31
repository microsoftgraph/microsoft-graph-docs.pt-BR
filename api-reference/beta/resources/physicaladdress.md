---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 35826dabd9052023abdc9d8c83ac9640ef550061
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966108"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="07acb-103">Tipo de recurso physicalAddress</span><span class="sxs-lookup"><span data-stu-id="07acb-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07acb-104">Representa o endereço físico de um recurso, como um contato ou evento.</span><span class="sxs-lookup"><span data-stu-id="07acb-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="07acb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07acb-105">Properties</span></span>
| <span data-ttu-id="07acb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07acb-106">Property</span></span>     | <span data-ttu-id="07acb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="07acb-107">Type</span></span>   |<span data-ttu-id="07acb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="07acb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07acb-109">city</span><span class="sxs-lookup"><span data-stu-id="07acb-109">city</span></span>|<span data-ttu-id="07acb-110">String</span><span class="sxs-lookup"><span data-stu-id="07acb-110">String</span></span>|<span data-ttu-id="07acb-111">A cidade.</span><span class="sxs-lookup"><span data-stu-id="07acb-111">The city.</span></span>|
|<span data-ttu-id="07acb-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="07acb-112">countryOrRegion</span></span>|<span data-ttu-id="07acb-113">String</span><span class="sxs-lookup"><span data-stu-id="07acb-113">String</span></span>|<span data-ttu-id="07acb-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="07acb-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="07acb-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="07acb-116">postalCode</span></span>|<span data-ttu-id="07acb-117">String</span><span class="sxs-lookup"><span data-stu-id="07acb-117">String</span></span>|<span data-ttu-id="07acb-118">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="07acb-118">The postal code.</span></span>|
|<span data-ttu-id="07acb-119">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="07acb-119">postOfficeBox</span></span>|<span data-ttu-id="07acb-120">String</span><span class="sxs-lookup"><span data-stu-id="07acb-120">String</span></span>|<span data-ttu-id="07acb-121">O número da caixa postal.</span><span class="sxs-lookup"><span data-stu-id="07acb-121">The post office box number.</span></span>|
|<span data-ttu-id="07acb-122">state</span><span class="sxs-lookup"><span data-stu-id="07acb-122">state</span></span>|<span data-ttu-id="07acb-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07acb-123">String</span></span>|<span data-ttu-id="07acb-124">O estado.</span><span class="sxs-lookup"><span data-stu-id="07acb-124">The state.</span></span>|
|<span data-ttu-id="07acb-125">street</span><span class="sxs-lookup"><span data-stu-id="07acb-125">street</span></span>|<span data-ttu-id="07acb-126">String</span><span class="sxs-lookup"><span data-stu-id="07acb-126">String</span></span>|<span data-ttu-id="07acb-127">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="07acb-127">The street.</span></span>|
|<span data-ttu-id="07acb-128">type</span><span class="sxs-lookup"><span data-stu-id="07acb-128">type</span></span>|<span data-ttu-id="07acb-129">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="07acb-129">physicalAddressType</span></span>|<span data-ttu-id="07acb-130">O tipo de endereço.</span><span class="sxs-lookup"><span data-stu-id="07acb-130">The type of address.</span></span> <span data-ttu-id="07acb-131">Os valores possíveis são: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="07acb-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="07acb-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07acb-132">JSON representation</span></span>

<span data-ttu-id="07acb-133">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="07acb-133">Here is a JSON representation of the resource</span></span>

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
