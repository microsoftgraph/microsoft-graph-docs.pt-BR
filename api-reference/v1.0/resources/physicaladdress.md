---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: kevinbellinger
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d9947e256001abd8168c886a0435e0725b3a1483
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072841"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="1921a-103">Tipo de recurso physicalAddress</span><span class="sxs-lookup"><span data-stu-id="1921a-103">physicalAddress resource type</span></span>

<span data-ttu-id="1921a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1921a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1921a-105">Representa o endereço físico de um recurso, como um contato ou evento.</span><span class="sxs-lookup"><span data-stu-id="1921a-105">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="1921a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1921a-106">Properties</span></span>
| <span data-ttu-id="1921a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1921a-107">Property</span></span>     | <span data-ttu-id="1921a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1921a-108">Type</span></span>   |<span data-ttu-id="1921a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1921a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1921a-110">city</span><span class="sxs-lookup"><span data-stu-id="1921a-110">city</span></span>|<span data-ttu-id="1921a-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1921a-111">String</span></span>|<span data-ttu-id="1921a-112">A cidade.</span><span class="sxs-lookup"><span data-stu-id="1921a-112">The city.</span></span>|
|<span data-ttu-id="1921a-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="1921a-113">countryOrRegion</span></span>|<span data-ttu-id="1921a-114">String</span><span class="sxs-lookup"><span data-stu-id="1921a-114">String</span></span>|<span data-ttu-id="1921a-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="1921a-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="1921a-117">postalCode</span><span class="sxs-lookup"><span data-stu-id="1921a-117">postalCode</span></span>|<span data-ttu-id="1921a-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1921a-118">String</span></span>|<span data-ttu-id="1921a-119">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="1921a-119">The postal code.</span></span>|
|<span data-ttu-id="1921a-120">state</span><span class="sxs-lookup"><span data-stu-id="1921a-120">state</span></span>|<span data-ttu-id="1921a-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1921a-121">String</span></span>|<span data-ttu-id="1921a-122">O estado.</span><span class="sxs-lookup"><span data-stu-id="1921a-122">The state.</span></span>|
|<span data-ttu-id="1921a-123">street</span><span class="sxs-lookup"><span data-stu-id="1921a-123">street</span></span>|<span data-ttu-id="1921a-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1921a-124">String</span></span>|<span data-ttu-id="1921a-125">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="1921a-125">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1921a-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1921a-126">JSON representation</span></span>

<span data-ttu-id="1921a-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1921a-127">Here is a JSON representation of the resource</span></span>

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
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

