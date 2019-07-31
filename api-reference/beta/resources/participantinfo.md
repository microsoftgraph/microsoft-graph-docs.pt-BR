---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ad73ce0bbeaa02b0207f11bbd3f0004857d90506
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966220"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="1ade2-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="1ade2-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ade2-104">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="1ade2-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="1ade2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ade2-105">Properties</span></span>

| <span data-ttu-id="1ade2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ade2-106">Property</span></span>       | <span data-ttu-id="1ade2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ade2-107">Type</span></span>                          | <span data-ttu-id="1ade2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ade2-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="1ade2-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="1ade2-109">identity</span></span>       | [<span data-ttu-id="1ade2-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="1ade2-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="1ade2-111">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="1ade2-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="1ade2-112">languageId</span><span class="sxs-lookup"><span data-stu-id="1ade2-112">languageId</span></span>     | <span data-ttu-id="1ade2-113">String</span><span class="sxs-lookup"><span data-stu-id="1ade2-113">String</span></span>                        | <span data-ttu-id="1ade2-114">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="1ade2-114">The language culture string.</span></span> |
| <span data-ttu-id="1ade2-115">região</span><span class="sxs-lookup"><span data-stu-id="1ade2-115">region</span></span>         | <span data-ttu-id="1ade2-116">String</span><span class="sxs-lookup"><span data-stu-id="1ade2-116">String</span></span>                        | <span data-ttu-id="1ade2-117">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="1ade2-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1ade2-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ade2-118">JSON representation</span></span>

<span data-ttu-id="1ade2-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ade2-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
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
