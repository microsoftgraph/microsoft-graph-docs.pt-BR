---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
ms.openlocfilehash: 3a656046cc23394fc8cff9100eb5ad2289050b25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823580"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="c34ae-103">Tipo de recurso physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c34ae-103">physicalAddress resource type</span></span>

<span data-ttu-id="c34ae-104">Representa o endereço físico de um recurso, como um contato ou evento.</span><span class="sxs-lookup"><span data-stu-id="c34ae-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="c34ae-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c34ae-105">Properties</span></span>
| <span data-ttu-id="c34ae-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c34ae-106">Property</span></span>     | <span data-ttu-id="c34ae-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c34ae-107">Type</span></span>   |<span data-ttu-id="c34ae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c34ae-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c34ae-109">type</span><span class="sxs-lookup"><span data-stu-id="c34ae-109">type</span></span>|<span data-ttu-id="c34ae-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c34ae-110">String</span></span>|<span data-ttu-id="c34ae-111">O tipo de endereço.</span><span class="sxs-lookup"><span data-stu-id="c34ae-111">The type of address.</span></span> <span data-ttu-id="c34ae-112">Os valores possíveis são: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="c34ae-112">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|
|<span data-ttu-id="c34ae-113">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="c34ae-113">postOfficeBox</span></span>|<span data-ttu-id="c34ae-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c34ae-114">String</span></span>|<span data-ttu-id="c34ae-115">O número de caixa postal.</span><span class="sxs-lookup"><span data-stu-id="c34ae-115">The post office box number.</span></span>|
|<span data-ttu-id="c34ae-116">city</span><span class="sxs-lookup"><span data-stu-id="c34ae-116">city</span></span>|<span data-ttu-id="c34ae-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c34ae-117">String</span></span>|<span data-ttu-id="c34ae-118">A cidade.</span><span class="sxs-lookup"><span data-stu-id="c34ae-118">The city.</span></span>|
|<span data-ttu-id="c34ae-119">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c34ae-119">countryOrRegion</span></span>|<span data-ttu-id="c34ae-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c34ae-120">String</span></span>|<span data-ttu-id="c34ae-p102">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="c34ae-p102">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="c34ae-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="c34ae-123">postalCode</span></span>|<span data-ttu-id="c34ae-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c34ae-124">String</span></span>|<span data-ttu-id="c34ae-125">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="c34ae-125">The postal code.</span></span>|
|<span data-ttu-id="c34ae-126">state</span><span class="sxs-lookup"><span data-stu-id="c34ae-126">state</span></span>|<span data-ttu-id="c34ae-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c34ae-127">String</span></span>|<span data-ttu-id="c34ae-128">O estado.</span><span class="sxs-lookup"><span data-stu-id="c34ae-128">The state.</span></span>|
|<span data-ttu-id="c34ae-129">street</span><span class="sxs-lookup"><span data-stu-id="c34ae-129">street</span></span>|<span data-ttu-id="c34ae-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c34ae-130">String</span></span>|<span data-ttu-id="c34ae-131">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="c34ae-131">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c34ae-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c34ae-132">JSON representation</span></span>

<span data-ttu-id="c34ae-133">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c34ae-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "type": "string",
  "postOfficeBox": "string",
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
