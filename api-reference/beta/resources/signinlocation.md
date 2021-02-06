---
title: Tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a login aconteceu.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: bc45d94896cbd822cdad4e3451f471bc3b540888
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134677"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="12cfc-103">Tipo de recurso signInLocation</span><span class="sxs-lookup"><span data-stu-id="12cfc-103">signInLocation resource type</span></span>

<span data-ttu-id="12cfc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12cfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12cfc-105">Fornece a cidade, o estado e o país/região de onde a login aconteceu.</span><span class="sxs-lookup"><span data-stu-id="12cfc-105">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="12cfc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12cfc-106">Properties</span></span>
| <span data-ttu-id="12cfc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12cfc-107">Property</span></span>     | <span data-ttu-id="12cfc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="12cfc-108">Type</span></span>   |<span data-ttu-id="12cfc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="12cfc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12cfc-110">city</span><span class="sxs-lookup"><span data-stu-id="12cfc-110">city</span></span>|<span data-ttu-id="12cfc-111">String</span><span class="sxs-lookup"><span data-stu-id="12cfc-111">String</span></span>|<span data-ttu-id="12cfc-112">Fornece a cidade de origem do login.</span><span class="sxs-lookup"><span data-stu-id="12cfc-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="12cfc-113">Isso é calculado usando informações de latitude/longitude da atividade de login.</span><span class="sxs-lookup"><span data-stu-id="12cfc-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="12cfc-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="12cfc-114">countryOrRegion</span></span>|<span data-ttu-id="12cfc-115">String</span><span class="sxs-lookup"><span data-stu-id="12cfc-115">String</span></span>|<span data-ttu-id="12cfc-116">Fornece as informações de código do país (código de 2 letras) onde a login se originou.</span><span class="sxs-lookup"><span data-stu-id="12cfc-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="12cfc-117">Isso é calculado usando informações de latitude/longitude da atividade de login.</span><span class="sxs-lookup"><span data-stu-id="12cfc-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="12cfc-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="12cfc-118">geoCoordinates</span></span>|[<span data-ttu-id="12cfc-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="12cfc-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="12cfc-120">Fornece a latitude, longitude e altitude de onde a login se originou.</span><span class="sxs-lookup"><span data-stu-id="12cfc-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="12cfc-121">estado</span><span class="sxs-lookup"><span data-stu-id="12cfc-121">state</span></span>|<span data-ttu-id="12cfc-122">String</span><span class="sxs-lookup"><span data-stu-id="12cfc-122">String</span></span>|<span data-ttu-id="12cfc-123">Fornece o estado de origem do login.</span><span class="sxs-lookup"><span data-stu-id="12cfc-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="12cfc-124">Isso é calculado usando informações de latitude/longitude da atividade de login.</span><span class="sxs-lookup"><span data-stu-id="12cfc-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12cfc-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12cfc-125">JSON representation</span></span>

<span data-ttu-id="12cfc-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12cfc-126">Here is a JSON representation of the resource.</span></span>

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


