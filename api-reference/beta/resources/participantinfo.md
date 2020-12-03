---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8c05222185b87e03c86257939cec098b3ac212e8
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522955"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="bb3dd-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="bb3dd-103">participantInfo resource type</span></span>

<span data-ttu-id="bb3dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb3dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb3dd-105">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="bb3dd-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="bb3dd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb3dd-106">Properties</span></span>

| <span data-ttu-id="bb3dd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb3dd-107">Property</span></span>         | <span data-ttu-id="bb3dd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb3dd-108">Type</span></span>                            | <span data-ttu-id="bb3dd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb3dd-109">Description</span></span>                                                                                                                                                                                                      |
| :--------------- | :------------------------------ | :-----------------------------------------------------------------------------------------------------------------------------------------------------------                                                     |
| <span data-ttu-id="bb3dd-110">countryCode</span><span class="sxs-lookup"><span data-stu-id="bb3dd-110">countryCode</span></span>      | <span data-ttu-id="bb3dd-111">String</span><span class="sxs-lookup"><span data-stu-id="bb3dd-111">String</span></span>                          | <span data-ttu-id="bb3dd-112">O código do país ISO 3166-1 alfa-2 do local físico mais estimado do participante no início da chamada.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-112">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="bb3dd-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-113">Read-only.</span></span>                                                                                   |
| <span data-ttu-id="bb3dd-114">EndpointType</span><span class="sxs-lookup"><span data-stu-id="bb3dd-114">endpointType</span></span>     | <span data-ttu-id="bb3dd-115">String</span><span class="sxs-lookup"><span data-stu-id="bb3dd-115">String</span></span>                          | <span data-ttu-id="bb3dd-116">O tipo de ponto de extremidade que o participante está usando.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-116">The type of endpoint the participant is using.</span></span> <span data-ttu-id="bb3dd-117">Os valores possíveis são: `default` , `skypeForBusiness` , ou `skypeForBusinessVoipPhone` .</span><span class="sxs-lookup"><span data-stu-id="bb3dd-117">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="bb3dd-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-118">Read-only.</span></span>                                                                    |
| <span data-ttu-id="bb3dd-119">ladrões</span><span class="sxs-lookup"><span data-stu-id="bb3dd-119">identity</span></span>         | [<span data-ttu-id="bb3dd-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="bb3dd-120">identitySet</span></span>](identityset.md)   | <span data-ttu-id="bb3dd-121">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-121">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="bb3dd-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-122">Read-only.</span></span>                                                                                                                                   |
| <span data-ttu-id="bb3dd-123">languageId</span><span class="sxs-lookup"><span data-stu-id="bb3dd-123">languageId</span></span>       | <span data-ttu-id="bb3dd-124">String</span><span class="sxs-lookup"><span data-stu-id="bb3dd-124">String</span></span>                          | <span data-ttu-id="bb3dd-125">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-125">The language culture string.</span></span> <span data-ttu-id="bb3dd-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-126">Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="bb3dd-127">região</span><span class="sxs-lookup"><span data-stu-id="bb3dd-127">region</span></span>           | <span data-ttu-id="bb3dd-128">String</span><span class="sxs-lookup"><span data-stu-id="bb3dd-128">String</span></span>                          | <span data-ttu-id="bb3dd-129">A região de início do participante.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-129">The home region of the participant.</span></span> <span data-ttu-id="bb3dd-130">Pode ser um país, um continente ou uma região geográfica maior.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-130">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="bb3dd-131">Isso não é alterado com base no local físico atual do participante, ao contrário do countryCode.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-131">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="bb3dd-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-132">Read-only.</span></span> |
| <span data-ttu-id="bb3dd-133">platformId</span><span class="sxs-lookup"><span data-stu-id="bb3dd-133">platformId</span></span>       | <span data-ttu-id="bb3dd-134">String</span><span class="sxs-lookup"><span data-stu-id="bb3dd-134">String</span></span>                          | <span data-ttu-id="bb3dd-135">A ID de plataforma do cliente do participante.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-135">The client platform ID of the participant.</span></span> <span data-ttu-id="bb3dd-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-136">Read-only.</span></span>    |


## <a name="json-representation"></a><span data-ttu-id="bb3dd-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb3dd-137">JSON representation</span></span>

<span data-ttu-id="bb3dd-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb3dd-138">The following is a JSON representation of the resource.</span></span>

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
  "region": "String",
  "platformId": "String",
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


