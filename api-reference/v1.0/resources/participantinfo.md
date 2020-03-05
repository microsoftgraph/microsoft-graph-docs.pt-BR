---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0316cb1bbe474f8265ed384774183759d29aca0f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447245"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="759bd-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="759bd-103">participantInfo resource type</span></span>

<span data-ttu-id="759bd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="759bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="759bd-105">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="759bd-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="759bd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="759bd-106">Properties</span></span>

| <span data-ttu-id="759bd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="759bd-107">Property</span></span>       | <span data-ttu-id="759bd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="759bd-108">Type</span></span>                          | <span data-ttu-id="759bd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="759bd-109">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="759bd-110">ladrões</span><span class="sxs-lookup"><span data-stu-id="759bd-110">identity</span></span>       | [<span data-ttu-id="759bd-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="759bd-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="759bd-112">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="759bd-112">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="759bd-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="759bd-113">Read-only.</span></span>                                                                             |
| <span data-ttu-id="759bd-114">languageId</span><span class="sxs-lookup"><span data-stu-id="759bd-114">languageId</span></span>     | <span data-ttu-id="759bd-115">String</span><span class="sxs-lookup"><span data-stu-id="759bd-115">String</span></span>                        | <span data-ttu-id="759bd-116">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="759bd-116">The language culture string.</span></span> <span data-ttu-id="759bd-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="759bd-117">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="759bd-118">região</span><span class="sxs-lookup"><span data-stu-id="759bd-118">region</span></span>         | <span data-ttu-id="759bd-119">String</span><span class="sxs-lookup"><span data-stu-id="759bd-119">String</span></span>                        | <span data-ttu-id="759bd-120">A região de início do participante.</span><span class="sxs-lookup"><span data-stu-id="759bd-120">The home region of the participant.</span></span> <span data-ttu-id="759bd-121">Pode ser um país, um continente ou uma região geográfica maior.</span><span class="sxs-lookup"><span data-stu-id="759bd-121">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="759bd-122">Isso não é alterado com base no local físico atual do participante.</span><span class="sxs-lookup"><span data-stu-id="759bd-122">This does not change based on the participant's current physical location.</span></span> <span data-ttu-id="759bd-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="759bd-123">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="759bd-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="759bd-124">JSON representation</span></span>

<span data-ttu-id="759bd-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="759bd-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId",
    "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
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
