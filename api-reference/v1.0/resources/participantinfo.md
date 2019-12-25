---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1dcc164769c2e8168be5f593c35cd62218254add
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870985"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="9694f-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="9694f-103">participantInfo resource type</span></span>

<span data-ttu-id="9694f-104">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="9694f-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="9694f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9694f-105">Properties</span></span>

| <span data-ttu-id="9694f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9694f-106">Property</span></span>       | <span data-ttu-id="9694f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9694f-107">Type</span></span>                          | <span data-ttu-id="9694f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9694f-108">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9694f-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="9694f-109">identity</span></span>       | [<span data-ttu-id="9694f-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="9694f-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="9694f-111">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="9694f-111">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="9694f-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9694f-112">Read-only.</span></span>                                                                             |
| <span data-ttu-id="9694f-113">languageId</span><span class="sxs-lookup"><span data-stu-id="9694f-113">languageId</span></span>     | <span data-ttu-id="9694f-114">String</span><span class="sxs-lookup"><span data-stu-id="9694f-114">String</span></span>                        | <span data-ttu-id="9694f-115">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="9694f-115">The language culture string.</span></span> <span data-ttu-id="9694f-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9694f-116">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="9694f-117">região</span><span class="sxs-lookup"><span data-stu-id="9694f-117">region</span></span>         | <span data-ttu-id="9694f-118">String</span><span class="sxs-lookup"><span data-stu-id="9694f-118">String</span></span>                        | <span data-ttu-id="9694f-119">A região de início do participante.</span><span class="sxs-lookup"><span data-stu-id="9694f-119">The home region of the participant.</span></span> <span data-ttu-id="9694f-120">Pode ser um país, um continente ou uma região geográfica maior.</span><span class="sxs-lookup"><span data-stu-id="9694f-120">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="9694f-121">Isso não é alterado com base no local físico atual do participante.</span><span class="sxs-lookup"><span data-stu-id="9694f-121">This does not change based on the participant's current physical location.</span></span> <span data-ttu-id="9694f-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9694f-122">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9694f-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9694f-123">JSON representation</span></span>

<span data-ttu-id="9694f-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9694f-124">The following is a JSON representation of the resource.</span></span>

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
