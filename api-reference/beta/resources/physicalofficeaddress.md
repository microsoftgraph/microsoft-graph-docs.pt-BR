---
title: tipo de recurso physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou um evento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 46bf87af658e0dc01c0f0db888118f7ae3bcde13
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997799"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="d3cf5-103">tipo de recurso physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="d3cf5-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="d3cf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3cf5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3cf5-105">Representa o endereço comercial de um recurso, como um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="d3cf5-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="d3cf5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3cf5-106">Properties</span></span>

| <span data-ttu-id="d3cf5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3cf5-107">Property</span></span>     | <span data-ttu-id="d3cf5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3cf5-108">Type</span></span>   |<span data-ttu-id="d3cf5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3cf5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3cf5-110">city</span><span class="sxs-lookup"><span data-stu-id="d3cf5-110">city</span></span>|<span data-ttu-id="d3cf5-111">String</span><span class="sxs-lookup"><span data-stu-id="d3cf5-111">String</span></span>|<span data-ttu-id="d3cf5-112">A cidade.</span><span class="sxs-lookup"><span data-stu-id="d3cf5-112">The city.</span></span>|
|<span data-ttu-id="d3cf5-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="d3cf5-113">countryOrRegion</span></span>|<span data-ttu-id="d3cf5-114">String</span><span class="sxs-lookup"><span data-stu-id="d3cf5-114">String</span></span>|<span data-ttu-id="d3cf5-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="d3cf5-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="d3cf5-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="d3cf5-117">officeLocation</span></span>  | <span data-ttu-id="d3cf5-118">String</span><span class="sxs-lookup"><span data-stu-id="d3cf5-118">String</span></span> | <span data-ttu-id="d3cf5-119">Local do Office, como o prédio e o número do escritório de um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="d3cf5-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="d3cf5-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="d3cf5-120">postalCode</span></span>|<span data-ttu-id="d3cf5-121">String</span><span class="sxs-lookup"><span data-stu-id="d3cf5-121">String</span></span>|<span data-ttu-id="d3cf5-122">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="d3cf5-122">The postal code.</span></span>|
|<span data-ttu-id="d3cf5-123">state</span><span class="sxs-lookup"><span data-stu-id="d3cf5-123">state</span></span>|<span data-ttu-id="d3cf5-124">String</span><span class="sxs-lookup"><span data-stu-id="d3cf5-124">String</span></span>|<span data-ttu-id="d3cf5-125">O estado.</span><span class="sxs-lookup"><span data-stu-id="d3cf5-125">The state.</span></span>|
|<span data-ttu-id="d3cf5-126">street</span><span class="sxs-lookup"><span data-stu-id="d3cf5-126">street</span></span>|<span data-ttu-id="d3cf5-127">String</span><span class="sxs-lookup"><span data-stu-id="d3cf5-127">String</span></span>|<span data-ttu-id="d3cf5-128">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="d3cf5-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3cf5-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3cf5-129">JSON representation</span></span>

<span data-ttu-id="d3cf5-130">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d3cf5-130">Here is a JSON representation of the resource</span></span>

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


