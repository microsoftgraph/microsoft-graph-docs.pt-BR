---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b48c8d9e8e2b7b39a63b919ff30178d8c8ac8536
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998240"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="706c6-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="706c6-103">participantInfo resource type</span></span>

<span data-ttu-id="706c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="706c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="706c6-105">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="706c6-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="706c6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="706c6-106">Properties</span></span>

| <span data-ttu-id="706c6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="706c6-107">Property</span></span>       | <span data-ttu-id="706c6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="706c6-108">Type</span></span>                          | <span data-ttu-id="706c6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="706c6-109">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="706c6-110">countryCode</span><span class="sxs-lookup"><span data-stu-id="706c6-110">countryCode</span></span>    | <span data-ttu-id="706c6-111">String</span><span class="sxs-lookup"><span data-stu-id="706c6-111">String</span></span>                        | <span data-ttu-id="706c6-112">O código do país ISO 3166-1 alfa-2 do local físico mais estimado do participante no início da chamada.</span><span class="sxs-lookup"><span data-stu-id="706c6-112">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="706c6-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706c6-113">Read-only.</span></span>                             |
| <span data-ttu-id="706c6-114">EndpointType</span><span class="sxs-lookup"><span data-stu-id="706c6-114">endpointType</span></span>   | <span data-ttu-id="706c6-115">String</span><span class="sxs-lookup"><span data-stu-id="706c6-115">String</span></span>                        | <span data-ttu-id="706c6-116">O tipo de ponto de extremidade que o participante está usando.</span><span class="sxs-lookup"><span data-stu-id="706c6-116">The type of endpoint the participant is using.</span></span> <span data-ttu-id="706c6-117">Os valores possíveis são: `default` , `skypeForBusiness` , ou `skypeForBusinessVoipPhone` .</span><span class="sxs-lookup"><span data-stu-id="706c6-117">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="706c6-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706c6-118">Read-only.</span></span>              |
| <span data-ttu-id="706c6-119">ladrões</span><span class="sxs-lookup"><span data-stu-id="706c6-119">identity</span></span>       | [<span data-ttu-id="706c6-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="706c6-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="706c6-121">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="706c6-121">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="706c6-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706c6-122">Read-only.</span></span>                                                                             |
| <span data-ttu-id="706c6-123">languageId</span><span class="sxs-lookup"><span data-stu-id="706c6-123">languageId</span></span>     | <span data-ttu-id="706c6-124">String</span><span class="sxs-lookup"><span data-stu-id="706c6-124">String</span></span>                        | <span data-ttu-id="706c6-125">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="706c6-125">The language culture string.</span></span> <span data-ttu-id="706c6-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706c6-126">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="706c6-127">região</span><span class="sxs-lookup"><span data-stu-id="706c6-127">region</span></span>         | <span data-ttu-id="706c6-128">String</span><span class="sxs-lookup"><span data-stu-id="706c6-128">String</span></span>                        | <span data-ttu-id="706c6-129">A região de início do participante.</span><span class="sxs-lookup"><span data-stu-id="706c6-129">The home region of the participant.</span></span> <span data-ttu-id="706c6-130">Pode ser um país, um continente ou uma região geográfica maior.</span><span class="sxs-lookup"><span data-stu-id="706c6-130">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="706c6-131">Isso não é alterado com base no local físico atual do participante, ao contrário do countryCode.</span><span class="sxs-lookup"><span data-stu-id="706c6-131">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="706c6-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706c6-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="706c6-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="706c6-133">JSON representation</span></span>

<span data-ttu-id="706c6-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="706c6-134">The following is a JSON representation of the resource.</span></span>

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


