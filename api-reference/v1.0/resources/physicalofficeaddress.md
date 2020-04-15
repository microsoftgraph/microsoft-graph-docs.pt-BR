---
title: tipo de recurso physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou um evento.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 46674ad9be3e86fd36f5a5beb52829959bbd340b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445543"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="cc167-103">tipo de recurso physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="cc167-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="cc167-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc167-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc167-105">Representa o endereço comercial de um recurso, como um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="cc167-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="cc167-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc167-106">Properties</span></span>

| <span data-ttu-id="cc167-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc167-107">Property</span></span>     | <span data-ttu-id="cc167-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc167-108">Type</span></span>   |<span data-ttu-id="cc167-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc167-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc167-110">city</span><span class="sxs-lookup"><span data-stu-id="cc167-110">city</span></span>|<span data-ttu-id="cc167-111">String</span><span class="sxs-lookup"><span data-stu-id="cc167-111">String</span></span>|<span data-ttu-id="cc167-112">A cidade.</span><span class="sxs-lookup"><span data-stu-id="cc167-112">The city.</span></span>|
|<span data-ttu-id="cc167-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="cc167-113">countryOrRegion</span></span>|<span data-ttu-id="cc167-114">String</span><span class="sxs-lookup"><span data-stu-id="cc167-114">String</span></span>|<span data-ttu-id="cc167-p101">O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".</span><span class="sxs-lookup"><span data-stu-id="cc167-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="cc167-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="cc167-117">officeLocation</span></span>  | <span data-ttu-id="cc167-118">String</span><span class="sxs-lookup"><span data-stu-id="cc167-118">String</span></span> | <span data-ttu-id="cc167-119">Local do Office, como o prédio e o número do escritório de um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="cc167-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="cc167-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="cc167-120">postalCode</span></span>|<span data-ttu-id="cc167-121">String</span><span class="sxs-lookup"><span data-stu-id="cc167-121">String</span></span>|<span data-ttu-id="cc167-122">O código de endereçamento postal, ou CEP.</span><span class="sxs-lookup"><span data-stu-id="cc167-122">The postal code.</span></span>|
|<span data-ttu-id="cc167-123">state</span><span class="sxs-lookup"><span data-stu-id="cc167-123">state</span></span>|<span data-ttu-id="cc167-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc167-124">String</span></span>|<span data-ttu-id="cc167-125">O estado.</span><span class="sxs-lookup"><span data-stu-id="cc167-125">The state.</span></span>|
|<span data-ttu-id="cc167-126">street</span><span class="sxs-lookup"><span data-stu-id="cc167-126">street</span></span>|<span data-ttu-id="cc167-127">String</span><span class="sxs-lookup"><span data-stu-id="cc167-127">String</span></span>|<span data-ttu-id="cc167-128">O tipo de logradouro (rua, alameda, avenida, etc.).</span><span class="sxs-lookup"><span data-stu-id="cc167-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc167-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc167-129">JSON representation</span></span>

<span data-ttu-id="cc167-130">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="cc167-130">Here is a JSON representation of the resource</span></span>

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
