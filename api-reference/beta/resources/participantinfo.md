---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: eea85cd861524ca947359918fd130c0dd221e146
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39637063"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="acabb-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="acabb-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acabb-104">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="acabb-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="acabb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acabb-105">Properties</span></span>

| <span data-ttu-id="acabb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acabb-106">Property</span></span>       | <span data-ttu-id="acabb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="acabb-107">Type</span></span>                          | <span data-ttu-id="acabb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="acabb-108">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="acabb-109">countryCode</span><span class="sxs-lookup"><span data-stu-id="acabb-109">countryCode</span></span>    | <span data-ttu-id="acabb-110">String</span><span class="sxs-lookup"><span data-stu-id="acabb-110">String</span></span>                        | <span data-ttu-id="acabb-111">O código do país ISO 3166-1 alfa-2 do local físico mais estimado do participante no início da chamada.</span><span class="sxs-lookup"><span data-stu-id="acabb-111">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="acabb-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acabb-112">Read-only.</span></span>                             |
| <span data-ttu-id="acabb-113">EndpointType</span><span class="sxs-lookup"><span data-stu-id="acabb-113">endpointType</span></span>   | <span data-ttu-id="acabb-114">String</span><span class="sxs-lookup"><span data-stu-id="acabb-114">String</span></span>                        | <span data-ttu-id="acabb-115">O tipo de ponto de extremidade que o participante está usando.</span><span class="sxs-lookup"><span data-stu-id="acabb-115">The type of endpoint the participant is using.</span></span> <span data-ttu-id="acabb-116">Os valores possíveis são `default`: `skypeForBusiness`,, `skypeForBusinessVoipPhone`ou.</span><span class="sxs-lookup"><span data-stu-id="acabb-116">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="acabb-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acabb-117">Read-only.</span></span>              |
| <span data-ttu-id="acabb-118">ladrões</span><span class="sxs-lookup"><span data-stu-id="acabb-118">identity</span></span>       | [<span data-ttu-id="acabb-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="acabb-119">identitySet</span></span>](identityset.md) | <span data-ttu-id="acabb-120">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="acabb-120">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="acabb-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acabb-121">Read-only.</span></span>                                                                             |
| <span data-ttu-id="acabb-122">languageId</span><span class="sxs-lookup"><span data-stu-id="acabb-122">languageId</span></span>     | <span data-ttu-id="acabb-123">String</span><span class="sxs-lookup"><span data-stu-id="acabb-123">String</span></span>                        | <span data-ttu-id="acabb-124">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="acabb-124">The language culture string.</span></span> <span data-ttu-id="acabb-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acabb-125">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="acabb-126">região</span><span class="sxs-lookup"><span data-stu-id="acabb-126">region</span></span>         | <span data-ttu-id="acabb-127">String</span><span class="sxs-lookup"><span data-stu-id="acabb-127">String</span></span>                        | <span data-ttu-id="acabb-128">A região de início do participante.</span><span class="sxs-lookup"><span data-stu-id="acabb-128">The home region of the participant.</span></span> <span data-ttu-id="acabb-129">Pode ser um país, um continente ou uma região geográfica maior.</span><span class="sxs-lookup"><span data-stu-id="acabb-129">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="acabb-130">Isso não é alterado com base no local físico atual do participante, ao contrário do countryCode.</span><span class="sxs-lookup"><span data-stu-id="acabb-130">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="acabb-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acabb-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="acabb-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acabb-132">JSON representation</span></span>

<span data-ttu-id="acabb-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acabb-133">The following is a JSON representation of the resource.</span></span>

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
