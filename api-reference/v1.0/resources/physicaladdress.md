---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
ms.openlocfilehash: eb2c1ea6a73d7f6eb5d3d43b877f50dc39a2b17e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005309"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="709a8-103">Tipo de recurso physicalAddress</span><span class="sxs-lookup"><span data-stu-id="709a8-103">physicalAddress resource type</span></span>

<span data-ttu-id="709a8-104">Representa o endereço físico de um recurso, como um contato ou evento.</span><span class="sxs-lookup"><span data-stu-id="709a8-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="709a8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="709a8-105">Properties</span></span>
| <span data-ttu-id="709a8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="709a8-106">Property</span></span>     | <span data-ttu-id="709a8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="709a8-107">Type</span></span>   |<span data-ttu-id="709a8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="709a8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="709a8-109">city</span><span class="sxs-lookup"><span data-stu-id="709a8-109">city</span></span>|<span data-ttu-id="709a8-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="709a8-110">String</span></span>|<span data-ttu-id="709a8-111">A cidade.</span><span class="sxs-lookup"><span data-stu-id="709a8-111">The city.</span></span>|
|<span data-ttu-id="709a8-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="709a8-112">countryOrRegion</span></span>|<span data-ttu-id="709a8-113">String</span><span class="sxs-lookup"><span data-stu-id="709a8-113">String</span></span>|<span data-ttu-id="709a8-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="709a8-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="709a8-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="709a8-116">postalCode</span></span>|<span data-ttu-id="709a8-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="709a8-117">String</span></span>|<span data-ttu-id="709a8-118">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="709a8-118">The postal code.</span></span>|
|<span data-ttu-id="709a8-119">state</span><span class="sxs-lookup"><span data-stu-id="709a8-119">state</span></span>|<span data-ttu-id="709a8-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="709a8-120">String</span></span>|<span data-ttu-id="709a8-121">O estado.</span><span class="sxs-lookup"><span data-stu-id="709a8-121">The state.</span></span>|
|<span data-ttu-id="709a8-122">street</span><span class="sxs-lookup"><span data-stu-id="709a8-122">street</span></span>|<span data-ttu-id="709a8-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="709a8-123">String</span></span>|<span data-ttu-id="709a8-124">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="709a8-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="709a8-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="709a8-125">JSON representation</span></span>

<span data-ttu-id="709a8-126">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="709a8-126">Here is a JSON representation of the resource</span></span>

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
