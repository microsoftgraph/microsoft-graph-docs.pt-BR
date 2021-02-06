---
title: Tipo de recurso physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou evento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: 8ff1672b0960c68ef826c89b9217109bdeb7da76
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130820"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="fa75f-103">Tipo de recurso physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="fa75f-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="fa75f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa75f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa75f-105">Representa o endereço comercial de um recurso, como um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="fa75f-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="fa75f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa75f-106">Properties</span></span>

| <span data-ttu-id="fa75f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa75f-107">Property</span></span>     | <span data-ttu-id="fa75f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa75f-108">Type</span></span>   |<span data-ttu-id="fa75f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa75f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa75f-110">city</span><span class="sxs-lookup"><span data-stu-id="fa75f-110">city</span></span>|<span data-ttu-id="fa75f-111">String</span><span class="sxs-lookup"><span data-stu-id="fa75f-111">String</span></span>|<span data-ttu-id="fa75f-112">A cidade.</span><span class="sxs-lookup"><span data-stu-id="fa75f-112">The city.</span></span>|
|<span data-ttu-id="fa75f-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="fa75f-113">countryOrRegion</span></span>|<span data-ttu-id="fa75f-114">String</span><span class="sxs-lookup"><span data-stu-id="fa75f-114">String</span></span>|<span data-ttu-id="fa75f-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="fa75f-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="fa75f-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="fa75f-117">officeLocation</span></span>  | <span data-ttu-id="fa75f-118">String</span><span class="sxs-lookup"><span data-stu-id="fa75f-118">String</span></span> | <span data-ttu-id="fa75f-119">Local do escritório, como prédio e número de escritório para um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="fa75f-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="fa75f-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="fa75f-120">postalCode</span></span>|<span data-ttu-id="fa75f-121">String</span><span class="sxs-lookup"><span data-stu-id="fa75f-121">String</span></span>|<span data-ttu-id="fa75f-122">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="fa75f-122">The postal code.</span></span>|
|<span data-ttu-id="fa75f-123">estado</span><span class="sxs-lookup"><span data-stu-id="fa75f-123">state</span></span>|<span data-ttu-id="fa75f-124">String</span><span class="sxs-lookup"><span data-stu-id="fa75f-124">String</span></span>|<span data-ttu-id="fa75f-125">O estado.</span><span class="sxs-lookup"><span data-stu-id="fa75f-125">The state.</span></span>|
|<span data-ttu-id="fa75f-126">street</span><span class="sxs-lookup"><span data-stu-id="fa75f-126">street</span></span>|<span data-ttu-id="fa75f-127">String</span><span class="sxs-lookup"><span data-stu-id="fa75f-127">String</span></span>|<span data-ttu-id="fa75f-128">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="fa75f-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa75f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa75f-129">JSON representation</span></span>

<span data-ttu-id="fa75f-130">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fa75f-130">Here is a JSON representation of the resource</span></span>

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


