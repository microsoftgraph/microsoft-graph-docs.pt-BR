---
title: tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a entrada ocorreu.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 58c3dc2b25b85963e6a0f6f88552dbf2a121d5f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446853"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="3a6fd-103">tipo de recurso signInLocation</span><span class="sxs-lookup"><span data-stu-id="3a6fd-103">signInLocation resource type</span></span>

<span data-ttu-id="3a6fd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3a6fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a6fd-105">Fornece a cidade, o estado e o país/região de onde a entrada ocorreu.</span><span class="sxs-lookup"><span data-stu-id="3a6fd-105">Provides the city, state and country/region from where the sign-in happened.</span></span>

## <a name="properties"></a><span data-ttu-id="3a6fd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a6fd-106">Properties</span></span>

| <span data-ttu-id="3a6fd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a6fd-107">Property</span></span>     | <span data-ttu-id="3a6fd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a6fd-108">Type</span></span>   |<span data-ttu-id="3a6fd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a6fd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a6fd-110">city</span><span class="sxs-lookup"><span data-stu-id="3a6fd-110">city</span></span>|<span data-ttu-id="3a6fd-111">String</span><span class="sxs-lookup"><span data-stu-id="3a6fd-111">String</span></span>|<span data-ttu-id="3a6fd-112">Fornece a cidade onde a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="3a6fd-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="3a6fd-113">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="3a6fd-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="3a6fd-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="3a6fd-114">countryOrRegion</span></span>|<span data-ttu-id="3a6fd-115">String</span><span class="sxs-lookup"><span data-stu-id="3a6fd-115">String</span></span>|<span data-ttu-id="3a6fd-116">Fornece as informações do código do país (código de 2 letras) em que a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="3a6fd-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="3a6fd-117">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="3a6fd-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="3a6fd-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3a6fd-118">geoCoordinates</span></span>|[<span data-ttu-id="3a6fd-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3a6fd-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="3a6fd-120">Fornece a latitude, longitude e altitude onde a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="3a6fd-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="3a6fd-121">state</span><span class="sxs-lookup"><span data-stu-id="3a6fd-121">state</span></span>|<span data-ttu-id="3a6fd-122">String</span><span class="sxs-lookup"><span data-stu-id="3a6fd-122">String</span></span>|<span data-ttu-id="3a6fd-123">Fornece o estado em que a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="3a6fd-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="3a6fd-124">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="3a6fd-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a6fd-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a6fd-125">JSON representation</span></span>

<span data-ttu-id="3a6fd-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a6fd-126">Here is a JSON representation of the resource.</span></span>

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
