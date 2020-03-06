---
title: tipo de recurso physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou um evento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0c7b0280d8b9e7d62357985b88ead034b015aef1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534061"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="80ba9-103">tipo de recurso physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="80ba9-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="80ba9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80ba9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80ba9-105">Representa o endereço comercial de um recurso, como um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="80ba9-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="80ba9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80ba9-106">Properties</span></span>

| <span data-ttu-id="80ba9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80ba9-107">Property</span></span>     | <span data-ttu-id="80ba9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="80ba9-108">Type</span></span>   |<span data-ttu-id="80ba9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="80ba9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80ba9-110">city</span><span class="sxs-lookup"><span data-stu-id="80ba9-110">city</span></span>|<span data-ttu-id="80ba9-111">String</span><span class="sxs-lookup"><span data-stu-id="80ba9-111">String</span></span>|<span data-ttu-id="80ba9-112">A cidade.</span><span class="sxs-lookup"><span data-stu-id="80ba9-112">The city.</span></span>|
|<span data-ttu-id="80ba9-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="80ba9-113">countryOrRegion</span></span>|<span data-ttu-id="80ba9-114">String</span><span class="sxs-lookup"><span data-stu-id="80ba9-114">String</span></span>|<span data-ttu-id="80ba9-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="80ba9-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="80ba9-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="80ba9-117">officeLocation</span></span>  | <span data-ttu-id="80ba9-118">String</span><span class="sxs-lookup"><span data-stu-id="80ba9-118">String</span></span> | <span data-ttu-id="80ba9-119">Local do Office, como o prédio e o número do escritório de um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="80ba9-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="80ba9-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="80ba9-120">postalCode</span></span>|<span data-ttu-id="80ba9-121">String</span><span class="sxs-lookup"><span data-stu-id="80ba9-121">String</span></span>|<span data-ttu-id="80ba9-122">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="80ba9-122">The postal code.</span></span>|
|<span data-ttu-id="80ba9-123">state</span><span class="sxs-lookup"><span data-stu-id="80ba9-123">state</span></span>|<span data-ttu-id="80ba9-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80ba9-124">String</span></span>|<span data-ttu-id="80ba9-125">O estado.</span><span class="sxs-lookup"><span data-stu-id="80ba9-125">The state.</span></span>|
|<span data-ttu-id="80ba9-126">street</span><span class="sxs-lookup"><span data-stu-id="80ba9-126">street</span></span>|<span data-ttu-id="80ba9-127">String</span><span class="sxs-lookup"><span data-stu-id="80ba9-127">String</span></span>|<span data-ttu-id="80ba9-128">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="80ba9-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80ba9-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80ba9-129">JSON representation</span></span>

<span data-ttu-id="80ba9-130">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="80ba9-130">Here is a JSON representation of the resource</span></span>

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
