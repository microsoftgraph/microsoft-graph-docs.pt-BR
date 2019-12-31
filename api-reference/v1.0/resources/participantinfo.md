---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9b603d93b2be2fef6a999cf3c1d7663fc7405da9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913727"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="d4f1c-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="d4f1c-103">participantInfo resource type</span></span>

<span data-ttu-id="d4f1c-104">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="d4f1c-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="d4f1c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4f1c-105">Properties</span></span>

| <span data-ttu-id="d4f1c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4f1c-106">Property</span></span>       | <span data-ttu-id="d4f1c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4f1c-107">Type</span></span>                          | <span data-ttu-id="d4f1c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4f1c-108">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d4f1c-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="d4f1c-109">identity</span></span>       | [<span data-ttu-id="d4f1c-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="d4f1c-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="d4f1c-111">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="d4f1c-111">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="d4f1c-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4f1c-112">Read-only.</span></span>                                                                             |
| <span data-ttu-id="d4f1c-113">languageId</span><span class="sxs-lookup"><span data-stu-id="d4f1c-113">languageId</span></span>     | <span data-ttu-id="d4f1c-114">String</span><span class="sxs-lookup"><span data-stu-id="d4f1c-114">String</span></span>                        | <span data-ttu-id="d4f1c-115">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="d4f1c-115">The language culture string.</span></span> <span data-ttu-id="d4f1c-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4f1c-116">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="d4f1c-117">região</span><span class="sxs-lookup"><span data-stu-id="d4f1c-117">region</span></span>         | <span data-ttu-id="d4f1c-118">String</span><span class="sxs-lookup"><span data-stu-id="d4f1c-118">String</span></span>                        | <span data-ttu-id="d4f1c-119">A região de início do participante.</span><span class="sxs-lookup"><span data-stu-id="d4f1c-119">The home region of the participant.</span></span> <span data-ttu-id="d4f1c-120">Pode ser um país, um continente ou uma região geográfica maior.</span><span class="sxs-lookup"><span data-stu-id="d4f1c-120">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="d4f1c-121">Isso não é alterado com base no local físico atual do participante.</span><span class="sxs-lookup"><span data-stu-id="d4f1c-121">This does not change based on the participant's current physical location.</span></span> <span data-ttu-id="d4f1c-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4f1c-122">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d4f1c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4f1c-123">JSON representation</span></span>

<span data-ttu-id="d4f1c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4f1c-124">The following is a JSON representation of the resource.</span></span>

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
