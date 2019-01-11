---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
ms.openlocfilehash: 2bbfc3f38d4d353d370b9c8ba859b06cc2e4398b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866007"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="457c6-103">Tipo de recurso physicalAddress</span><span class="sxs-lookup"><span data-stu-id="457c6-103">physicalAddress resource type</span></span>

<span data-ttu-id="457c6-104">Representa o endereço físico de um recurso, como um contato ou evento.</span><span class="sxs-lookup"><span data-stu-id="457c6-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="457c6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="457c6-105">Properties</span></span>
| <span data-ttu-id="457c6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="457c6-106">Property</span></span>     | <span data-ttu-id="457c6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="457c6-107">Type</span></span>   |<span data-ttu-id="457c6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="457c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="457c6-109">city</span><span class="sxs-lookup"><span data-stu-id="457c6-109">city</span></span>|<span data-ttu-id="457c6-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="457c6-110">String</span></span>|<span data-ttu-id="457c6-111">A cidade.</span><span class="sxs-lookup"><span data-stu-id="457c6-111">The city.</span></span>|
|<span data-ttu-id="457c6-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="457c6-112">countryOrRegion</span></span>|<span data-ttu-id="457c6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="457c6-113">String</span></span>|<span data-ttu-id="457c6-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="457c6-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="457c6-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="457c6-116">postalCode</span></span>|<span data-ttu-id="457c6-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="457c6-117">String</span></span>|<span data-ttu-id="457c6-118">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="457c6-118">The postal code.</span></span>|
|<span data-ttu-id="457c6-119">state</span><span class="sxs-lookup"><span data-stu-id="457c6-119">state</span></span>|<span data-ttu-id="457c6-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="457c6-120">String</span></span>|<span data-ttu-id="457c6-121">O estado.</span><span class="sxs-lookup"><span data-stu-id="457c6-121">The state.</span></span>|
|<span data-ttu-id="457c6-122">street</span><span class="sxs-lookup"><span data-stu-id="457c6-122">street</span></span>|<span data-ttu-id="457c6-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="457c6-123">String</span></span>|<span data-ttu-id="457c6-124">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="457c6-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="457c6-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="457c6-125">JSON representation</span></span>

<span data-ttu-id="457c6-126">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="457c6-126">Here is a JSON representation of the resource</span></span>

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
