---
title: Tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a login aconteceu.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c003fda44e54bbee5957e794d02b90f008f4b8f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137092"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="4a5c9-103">Tipo de recurso signInLocation</span><span class="sxs-lookup"><span data-stu-id="4a5c9-103">signInLocation resource type</span></span>

<span data-ttu-id="4a5c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a5c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a5c9-105">Fornece a cidade, o estado e o país/região de onde a login aconteceu.</span><span class="sxs-lookup"><span data-stu-id="4a5c9-105">Provides the city, state and country/region from where the sign-in happened.</span></span>

## <a name="properties"></a><span data-ttu-id="4a5c9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a5c9-106">Properties</span></span>

| <span data-ttu-id="4a5c9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a5c9-107">Property</span></span>     | <span data-ttu-id="4a5c9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a5c9-108">Type</span></span>   |<span data-ttu-id="4a5c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a5c9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a5c9-110">city</span><span class="sxs-lookup"><span data-stu-id="4a5c9-110">city</span></span>|<span data-ttu-id="4a5c9-111">String</span><span class="sxs-lookup"><span data-stu-id="4a5c9-111">String</span></span>|<span data-ttu-id="4a5c9-112">Fornece a cidade de origem do login.</span><span class="sxs-lookup"><span data-stu-id="4a5c9-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="4a5c9-113">Isso é calculado usando informações de latitude/longitude da atividade de login.</span><span class="sxs-lookup"><span data-stu-id="4a5c9-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="4a5c9-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="4a5c9-114">countryOrRegion</span></span>|<span data-ttu-id="4a5c9-115">String</span><span class="sxs-lookup"><span data-stu-id="4a5c9-115">String</span></span>|<span data-ttu-id="4a5c9-116">Fornece as informações de código do país (código de 2 letras) de origem do login.</span><span class="sxs-lookup"><span data-stu-id="4a5c9-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="4a5c9-117">Isso é calculado usando informações de latitude/longitude da atividade de login.</span><span class="sxs-lookup"><span data-stu-id="4a5c9-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="4a5c9-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="4a5c9-118">geoCoordinates</span></span>|[<span data-ttu-id="4a5c9-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="4a5c9-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="4a5c9-120">Fornece a latitude, longitude e altitude de onde a login se originou.</span><span class="sxs-lookup"><span data-stu-id="4a5c9-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="4a5c9-121">estado</span><span class="sxs-lookup"><span data-stu-id="4a5c9-121">state</span></span>|<span data-ttu-id="4a5c9-122">String</span><span class="sxs-lookup"><span data-stu-id="4a5c9-122">String</span></span>|<span data-ttu-id="4a5c9-123">Fornece o estado de origem do login.</span><span class="sxs-lookup"><span data-stu-id="4a5c9-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="4a5c9-124">Isso é calculado usando informações de latitude/longitude da atividade de login.</span><span class="sxs-lookup"><span data-stu-id="4a5c9-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a5c9-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a5c9-125">JSON representation</span></span>

<span data-ttu-id="4a5c9-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a5c9-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

