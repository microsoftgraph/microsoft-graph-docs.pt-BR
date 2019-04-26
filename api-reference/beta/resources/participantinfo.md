---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3d040fd5be86068c30e7a63dae50888c4f3ec756
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568563"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="0d22f-103">tipo de recurso participantInfo</span><span class="sxs-lookup"><span data-stu-id="0d22f-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d22f-104">Contém propriedades adicionais sobre a identidade do participante</span><span class="sxs-lookup"><span data-stu-id="0d22f-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="0d22f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d22f-105">Properties</span></span>

| <span data-ttu-id="0d22f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d22f-106">Property</span></span>       | <span data-ttu-id="0d22f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d22f-107">Type</span></span>                          | <span data-ttu-id="0d22f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d22f-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="0d22f-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="0d22f-109">identity</span></span>       | [<span data-ttu-id="0d22f-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="0d22f-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="0d22f-111">O [identityset](identityset.md) associado a este participante.</span><span class="sxs-lookup"><span data-stu-id="0d22f-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="0d22f-112">languageId</span><span class="sxs-lookup"><span data-stu-id="0d22f-112">languageId</span></span>     | <span data-ttu-id="0d22f-113">String</span><span class="sxs-lookup"><span data-stu-id="0d22f-113">String</span></span>                        | <span data-ttu-id="0d22f-114">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="0d22f-114">The language culture string.</span></span> |
| <span data-ttu-id="0d22f-115">região</span><span class="sxs-lookup"><span data-stu-id="0d22f-115">region</span></span>         | <span data-ttu-id="0d22f-116">String</span><span class="sxs-lookup"><span data-stu-id="0d22f-116">String</span></span>                        | <span data-ttu-id="0d22f-117">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="0d22f-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0d22f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d22f-118">JSON representation</span></span>

<span data-ttu-id="0d22f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d22f-119">The following is a JSON representation of the resource.</span></span>

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
