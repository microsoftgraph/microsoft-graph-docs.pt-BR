---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b3d8671c33a0040fde8671a2d97b67dae0e94b28
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913580"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="492b2-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="492b2-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="492b2-104">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="492b2-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="492b2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="492b2-105">Properties</span></span>

| <span data-ttu-id="492b2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="492b2-106">Property</span></span>       | <span data-ttu-id="492b2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="492b2-107">Type</span></span>                          | <span data-ttu-id="492b2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="492b2-108">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="492b2-109">countryCode</span><span class="sxs-lookup"><span data-stu-id="492b2-109">countryCode</span></span>    | <span data-ttu-id="492b2-110">String</span><span class="sxs-lookup"><span data-stu-id="492b2-110">String</span></span>                        | <span data-ttu-id="492b2-111">O código do país ISO 3166-1 alfa-2 do local físico mais estimado do participante no início da chamada.</span><span class="sxs-lookup"><span data-stu-id="492b2-111">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="492b2-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="492b2-112">Read-only.</span></span>                             |
| <span data-ttu-id="492b2-113">EndpointType</span><span class="sxs-lookup"><span data-stu-id="492b2-113">endpointType</span></span>   | <span data-ttu-id="492b2-114">String</span><span class="sxs-lookup"><span data-stu-id="492b2-114">String</span></span>                        | <span data-ttu-id="492b2-115">O tipo de ponto de extremidade que o participante está usando.</span><span class="sxs-lookup"><span data-stu-id="492b2-115">The type of endpoint the participant is using.</span></span> <span data-ttu-id="492b2-116">Os valores possíveis são `default`: `skypeForBusiness`,, `skypeForBusinessVoipPhone`ou.</span><span class="sxs-lookup"><span data-stu-id="492b2-116">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="492b2-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="492b2-117">Read-only.</span></span>              |
| <span data-ttu-id="492b2-118">ladrões</span><span class="sxs-lookup"><span data-stu-id="492b2-118">identity</span></span>       | [<span data-ttu-id="492b2-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="492b2-119">identitySet</span></span>](identityset.md) | <span data-ttu-id="492b2-120">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="492b2-120">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="492b2-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="492b2-121">Read-only.</span></span>                                                                             |
| <span data-ttu-id="492b2-122">languageId</span><span class="sxs-lookup"><span data-stu-id="492b2-122">languageId</span></span>     | <span data-ttu-id="492b2-123">String</span><span class="sxs-lookup"><span data-stu-id="492b2-123">String</span></span>                        | <span data-ttu-id="492b2-124">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="492b2-124">The language culture string.</span></span> <span data-ttu-id="492b2-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="492b2-125">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="492b2-126">região</span><span class="sxs-lookup"><span data-stu-id="492b2-126">region</span></span>         | <span data-ttu-id="492b2-127">String</span><span class="sxs-lookup"><span data-stu-id="492b2-127">String</span></span>                        | <span data-ttu-id="492b2-128">A região de início do participante.</span><span class="sxs-lookup"><span data-stu-id="492b2-128">The home region of the participant.</span></span> <span data-ttu-id="492b2-129">Pode ser um país, um continente ou uma região geográfica maior.</span><span class="sxs-lookup"><span data-stu-id="492b2-129">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="492b2-130">Isso não é alterado com base no local físico atual do participante, ao contrário do countryCode.</span><span class="sxs-lookup"><span data-stu-id="492b2-130">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="492b2-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="492b2-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="492b2-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="492b2-132">JSON representation</span></span>

<span data-ttu-id="492b2-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="492b2-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "countryCode",
    "endpointType",
    "languageId",
    "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "countryCode": "String",
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "endpointType": "default | skypeForBusiness | skypeForBusinessVoipPhone",
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
