---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9869cf1154735742630edf75ea3e4d5303d45bc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344908"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="edc2f-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="edc2f-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edc2f-104">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="edc2f-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="edc2f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="edc2f-105">Properties</span></span>

| <span data-ttu-id="edc2f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edc2f-106">Property</span></span>       | <span data-ttu-id="edc2f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="edc2f-107">Type</span></span>                          | <span data-ttu-id="edc2f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="edc2f-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="edc2f-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="edc2f-109">identity</span></span>       | [<span data-ttu-id="edc2f-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="edc2f-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="edc2f-111">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="edc2f-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="edc2f-112">languageId</span><span class="sxs-lookup"><span data-stu-id="edc2f-112">languageId</span></span>     | <span data-ttu-id="edc2f-113">String</span><span class="sxs-lookup"><span data-stu-id="edc2f-113">String</span></span>                        | <span data-ttu-id="edc2f-114">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="edc2f-114">The language culture string.</span></span> |
| <span data-ttu-id="edc2f-115">região</span><span class="sxs-lookup"><span data-stu-id="edc2f-115">region</span></span>         | <span data-ttu-id="edc2f-116">String</span><span class="sxs-lookup"><span data-stu-id="edc2f-116">String</span></span>                        | <span data-ttu-id="edc2f-117">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="edc2f-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="edc2f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="edc2f-118">JSON representation</span></span>

<span data-ttu-id="edc2f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="edc2f-119">The following is a JSON representation of the resource.</span></span>

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
