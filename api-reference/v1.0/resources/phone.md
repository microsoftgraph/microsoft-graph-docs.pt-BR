---
title: Tipo de recurso phone
description: Representa um número de telefone.
ms.openlocfilehash: 1293b1f84d9e73f5d92c9b6f6b078b5f39126e33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006415"
---
# <a name="phone-resource-type"></a><span data-ttu-id="c7456-103">Tipo de recurso phone</span><span class="sxs-lookup"><span data-stu-id="c7456-103">phone resource type</span></span>

<span data-ttu-id="c7456-104">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c7456-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="c7456-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7456-105">Properties</span></span>
| <span data-ttu-id="c7456-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7456-106">Property</span></span>     | <span data-ttu-id="c7456-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7456-107">Type</span></span>   |<span data-ttu-id="c7456-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7456-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7456-109">number</span><span class="sxs-lookup"><span data-stu-id="c7456-109">number</span></span>|<span data-ttu-id="c7456-110">string</span><span class="sxs-lookup"><span data-stu-id="c7456-110">string</span></span>|<span data-ttu-id="c7456-111">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c7456-111">The phone number.</span></span>|
|<span data-ttu-id="c7456-112">type</span><span class="sxs-lookup"><span data-stu-id="c7456-112">type</span></span>|<span data-ttu-id="c7456-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="c7456-113">phoneType</span></span>|<span data-ttu-id="c7456-114">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c7456-114">The type of phone number.</span></span> <span data-ttu-id="c7456-115">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="c7456-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7456-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7456-116">JSON representation</span></span>

<span data-ttu-id="c7456-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7456-117">Here is a JSON representation of the resource.</span></span>

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
