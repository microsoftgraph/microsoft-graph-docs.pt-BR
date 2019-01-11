---
title: Tipo de recurso phone
description: Representa um número de telefone.
localization_priority: Normal
ms.openlocfilehash: 6c34033b0895f81619589e7500441fc655842995
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805058"
---
# <a name="phone-resource-type"></a><span data-ttu-id="37500-103">Tipo de recurso phone</span><span class="sxs-lookup"><span data-stu-id="37500-103">phone resource type</span></span>

<span data-ttu-id="37500-104">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="37500-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="37500-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37500-105">Properties</span></span>
| <span data-ttu-id="37500-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37500-106">Property</span></span>     | <span data-ttu-id="37500-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="37500-107">Type</span></span>   |<span data-ttu-id="37500-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="37500-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37500-109">number</span><span class="sxs-lookup"><span data-stu-id="37500-109">number</span></span>|<span data-ttu-id="37500-110">string</span><span class="sxs-lookup"><span data-stu-id="37500-110">string</span></span>|<span data-ttu-id="37500-111">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="37500-111">The phone number.</span></span>|
|<span data-ttu-id="37500-112">type</span><span class="sxs-lookup"><span data-stu-id="37500-112">type</span></span>|<span data-ttu-id="37500-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="37500-113">phoneType</span></span>|<span data-ttu-id="37500-114">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="37500-114">The type of phone number.</span></span> <span data-ttu-id="37500-115">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="37500-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37500-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37500-116">JSON representation</span></span>

<span data-ttu-id="37500-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37500-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
