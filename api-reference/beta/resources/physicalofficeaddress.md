---
title: tipo de recurso de physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou evento.
localization_priority: Normal
ms.openlocfilehash: bd4274e29b2ef0f9e7e8318528d18103be19fabc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817784"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="475ce-103">tipo de recurso de physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="475ce-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="475ce-104">Representa o endereço comercial de um recurso, como um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="475ce-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="475ce-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="475ce-105">Properties</span></span>

| <span data-ttu-id="475ce-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="475ce-106">Property</span></span>     | <span data-ttu-id="475ce-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="475ce-107">Type</span></span>   |<span data-ttu-id="475ce-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="475ce-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="475ce-109">city</span><span class="sxs-lookup"><span data-stu-id="475ce-109">city</span></span>|<span data-ttu-id="475ce-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475ce-110">String</span></span>|<span data-ttu-id="475ce-111">A cidade.</span><span class="sxs-lookup"><span data-stu-id="475ce-111">The city.</span></span>|
|<span data-ttu-id="475ce-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="475ce-112">countryOrRegion</span></span>|<span data-ttu-id="475ce-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475ce-113">String</span></span>|<span data-ttu-id="475ce-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="475ce-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="475ce-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="475ce-116">officeLocation</span></span>  | <span data-ttu-id="475ce-117">String</span><span class="sxs-lookup"><span data-stu-id="475ce-117">String</span></span> | <span data-ttu-id="475ce-118">Local do escritório, como número de construção e do office para um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="475ce-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="475ce-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="475ce-119">postalCode</span></span>|<span data-ttu-id="475ce-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475ce-120">String</span></span>|<span data-ttu-id="475ce-121">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="475ce-121">The postal code.</span></span>|
|<span data-ttu-id="475ce-122">state</span><span class="sxs-lookup"><span data-stu-id="475ce-122">state</span></span>|<span data-ttu-id="475ce-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475ce-123">String</span></span>|<span data-ttu-id="475ce-124">O estado.</span><span class="sxs-lookup"><span data-stu-id="475ce-124">The state.</span></span>|
|<span data-ttu-id="475ce-125">street</span><span class="sxs-lookup"><span data-stu-id="475ce-125">street</span></span>|<span data-ttu-id="475ce-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475ce-126">String</span></span>|<span data-ttu-id="475ce-127">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="475ce-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="475ce-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="475ce-128">JSON representation</span></span>

<span data-ttu-id="475ce-129">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="475ce-129">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
