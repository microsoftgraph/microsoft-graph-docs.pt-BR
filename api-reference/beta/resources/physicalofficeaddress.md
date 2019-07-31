---
title: tipo de recurso physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou um evento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8299f72032cfb7910583fcd4dbefe914f054648e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966094"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="f7d78-103">tipo de recurso physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="f7d78-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="f7d78-104">Representa o endereço comercial de um recurso, como um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="f7d78-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="f7d78-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7d78-105">Properties</span></span>

| <span data-ttu-id="f7d78-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7d78-106">Property</span></span>     | <span data-ttu-id="f7d78-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7d78-107">Type</span></span>   |<span data-ttu-id="f7d78-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7d78-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7d78-109">city</span><span class="sxs-lookup"><span data-stu-id="f7d78-109">city</span></span>|<span data-ttu-id="f7d78-110">String</span><span class="sxs-lookup"><span data-stu-id="f7d78-110">String</span></span>|<span data-ttu-id="f7d78-111">A cidade.</span><span class="sxs-lookup"><span data-stu-id="f7d78-111">The city.</span></span>|
|<span data-ttu-id="f7d78-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="f7d78-112">countryOrRegion</span></span>|<span data-ttu-id="f7d78-113">String</span><span class="sxs-lookup"><span data-stu-id="f7d78-113">String</span></span>|<span data-ttu-id="f7d78-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="f7d78-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="f7d78-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="f7d78-116">officeLocation</span></span>  | <span data-ttu-id="f7d78-117">String</span><span class="sxs-lookup"><span data-stu-id="f7d78-117">String</span></span> | <span data-ttu-id="f7d78-118">Local do Office, como o prédio e o número do escritório de um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="f7d78-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="f7d78-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="f7d78-119">postalCode</span></span>|<span data-ttu-id="f7d78-120">String</span><span class="sxs-lookup"><span data-stu-id="f7d78-120">String</span></span>|<span data-ttu-id="f7d78-121">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="f7d78-121">The postal code.</span></span>|
|<span data-ttu-id="f7d78-122">state</span><span class="sxs-lookup"><span data-stu-id="f7d78-122">state</span></span>|<span data-ttu-id="f7d78-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7d78-123">String</span></span>|<span data-ttu-id="f7d78-124">O estado.</span><span class="sxs-lookup"><span data-stu-id="f7d78-124">The state.</span></span>|
|<span data-ttu-id="f7d78-125">street</span><span class="sxs-lookup"><span data-stu-id="f7d78-125">street</span></span>|<span data-ttu-id="f7d78-126">String</span><span class="sxs-lookup"><span data-stu-id="f7d78-126">String</span></span>|<span data-ttu-id="f7d78-127">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="f7d78-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7d78-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7d78-128">JSON representation</span></span>

<span data-ttu-id="f7d78-129">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f7d78-129">Here is a JSON representation of the resource</span></span>

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
