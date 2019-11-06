---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4cffe361b63ddc6d54d2ad16c29d2de8836044fc
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006589"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="f46ab-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="f46ab-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f46ab-104">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="f46ab-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="f46ab-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f46ab-105">Properties</span></span>

| <span data-ttu-id="f46ab-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f46ab-106">Property</span></span>       | <span data-ttu-id="f46ab-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f46ab-107">Type</span></span>                          | <span data-ttu-id="f46ab-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f46ab-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="f46ab-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="f46ab-109">identity</span></span>       | [<span data-ttu-id="f46ab-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="f46ab-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="f46ab-111">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="f46ab-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="f46ab-112">languageId</span><span class="sxs-lookup"><span data-stu-id="f46ab-112">languageId</span></span>     | <span data-ttu-id="f46ab-113">String</span><span class="sxs-lookup"><span data-stu-id="f46ab-113">String</span></span>                        | <span data-ttu-id="f46ab-114">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="f46ab-114">The language culture string.</span></span> |
| <span data-ttu-id="f46ab-115">região</span><span class="sxs-lookup"><span data-stu-id="f46ab-115">region</span></span>         | <span data-ttu-id="f46ab-116">String</span><span class="sxs-lookup"><span data-stu-id="f46ab-116">String</span></span>                        | <span data-ttu-id="f46ab-117">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="f46ab-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f46ab-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f46ab-118">JSON representation</span></span>

<span data-ttu-id="f46ab-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f46ab-119">The following is a JSON representation of the resource.</span></span>

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
