---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bd9c57961bee93e7d01e504bccb8671a8f1dd449
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522029"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="35eb2-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="35eb2-103">participantInfo resource type</span></span>

<span data-ttu-id="35eb2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="35eb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35eb2-105">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="35eb2-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="35eb2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35eb2-106">Properties</span></span>

| <span data-ttu-id="35eb2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35eb2-107">Property</span></span>       | <span data-ttu-id="35eb2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="35eb2-108">Type</span></span>                          | <span data-ttu-id="35eb2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="35eb2-109">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="35eb2-110">countryCode</span><span class="sxs-lookup"><span data-stu-id="35eb2-110">countryCode</span></span>    | <span data-ttu-id="35eb2-111">String</span><span class="sxs-lookup"><span data-stu-id="35eb2-111">String</span></span>                        | <span data-ttu-id="35eb2-112">O código do país ISO 3166-1 alfa-2 do local físico mais estimado do participante no início da chamada.</span><span class="sxs-lookup"><span data-stu-id="35eb2-112">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="35eb2-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35eb2-113">Read-only.</span></span>                             |
| <span data-ttu-id="35eb2-114">EndpointType</span><span class="sxs-lookup"><span data-stu-id="35eb2-114">endpointType</span></span>   | <span data-ttu-id="35eb2-115">String</span><span class="sxs-lookup"><span data-stu-id="35eb2-115">String</span></span>                        | <span data-ttu-id="35eb2-116">O tipo de ponto de extremidade que o participante está usando.</span><span class="sxs-lookup"><span data-stu-id="35eb2-116">The type of endpoint the participant is using.</span></span> <span data-ttu-id="35eb2-117">Os valores possíveis são `default`: `skypeForBusiness`,, `skypeForBusinessVoipPhone`ou.</span><span class="sxs-lookup"><span data-stu-id="35eb2-117">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="35eb2-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35eb2-118">Read-only.</span></span>              |
| <span data-ttu-id="35eb2-119">ladrões</span><span class="sxs-lookup"><span data-stu-id="35eb2-119">identity</span></span>       | [<span data-ttu-id="35eb2-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="35eb2-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="35eb2-121">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="35eb2-121">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="35eb2-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35eb2-122">Read-only.</span></span>                                                                             |
| <span data-ttu-id="35eb2-123">languageId</span><span class="sxs-lookup"><span data-stu-id="35eb2-123">languageId</span></span>     | <span data-ttu-id="35eb2-124">String</span><span class="sxs-lookup"><span data-stu-id="35eb2-124">String</span></span>                        | <span data-ttu-id="35eb2-125">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="35eb2-125">The language culture string.</span></span> <span data-ttu-id="35eb2-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35eb2-126">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="35eb2-127">região</span><span class="sxs-lookup"><span data-stu-id="35eb2-127">region</span></span>         | <span data-ttu-id="35eb2-128">String</span><span class="sxs-lookup"><span data-stu-id="35eb2-128">String</span></span>                        | <span data-ttu-id="35eb2-129">A região de início do participante.</span><span class="sxs-lookup"><span data-stu-id="35eb2-129">The home region of the participant.</span></span> <span data-ttu-id="35eb2-130">Pode ser um país, um continente ou uma região geográfica maior.</span><span class="sxs-lookup"><span data-stu-id="35eb2-130">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="35eb2-131">Isso não é alterado com base no local físico atual do participante, ao contrário do countryCode.</span><span class="sxs-lookup"><span data-stu-id="35eb2-131">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="35eb2-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35eb2-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35eb2-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35eb2-133">JSON representation</span></span>

<span data-ttu-id="35eb2-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35eb2-134">The following is a JSON representation of the resource.</span></span>

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
