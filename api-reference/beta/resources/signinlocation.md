---
title: tipo de recurso de signInLocation
description: Fornece a cidade, estado e país/região de onde a entrar aconteceu.
ms.openlocfilehash: a3d4f6ca5ec18e70960f45a3da1bb06d51ee1e65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037238"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="d5506-103">tipo de recurso de signInLocation</span><span class="sxs-lookup"><span data-stu-id="d5506-103">signInLocation resource type</span></span>
<span data-ttu-id="d5506-104">Fornece a cidade, estado e país/região de onde a entrar aconteceu.</span><span class="sxs-lookup"><span data-stu-id="d5506-104">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="d5506-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5506-105">Properties</span></span>
| <span data-ttu-id="d5506-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5506-106">Property</span></span>     | <span data-ttu-id="d5506-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5506-107">Type</span></span>   |<span data-ttu-id="d5506-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5506-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5506-109">city</span><span class="sxs-lookup"><span data-stu-id="d5506-109">city</span></span>|<span data-ttu-id="d5506-110">String</span><span class="sxs-lookup"><span data-stu-id="d5506-110">String</span></span>|<span data-ttu-id="d5506-111">Fornece a cidade onde o sign-in se originou.</span><span class="sxs-lookup"><span data-stu-id="d5506-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="d5506-112">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="d5506-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="d5506-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="d5506-113">countryOrRegion</span></span>|<span data-ttu-id="d5506-114">String</span><span class="sxs-lookup"><span data-stu-id="d5506-114">String</span></span>|<span data-ttu-id="d5506-115">Fornece as informações de código de país (código de carta 2) onde o sign-in se originou.</span><span class="sxs-lookup"><span data-stu-id="d5506-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="d5506-116">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="d5506-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="d5506-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d5506-117">geoCoordinates</span></span>|[<span data-ttu-id="d5506-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d5506-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="d5506-119">Fornece o latitude, longitude e altitude onde a entrar se originou.</span><span class="sxs-lookup"><span data-stu-id="d5506-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="d5506-120">state</span><span class="sxs-lookup"><span data-stu-id="d5506-120">state</span></span>|<span data-ttu-id="d5506-121">String</span><span class="sxs-lookup"><span data-stu-id="d5506-121">String</span></span>|<span data-ttu-id="d5506-122">Fornece o estado em que a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="d5506-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="d5506-123">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="d5506-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5506-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5506-124">JSON representation</span></span>

<span data-ttu-id="d5506-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5506-125">Here is a JSON representation of the resource.</span></span>

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