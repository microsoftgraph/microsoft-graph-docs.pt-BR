---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6bdcc4331b14ad7a0e03404781014b66daf55b46
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035473"
---
# <a name="phone-resource-type"></a><span data-ttu-id="906f1-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="906f1-103">phone resource type</span></span>

<span data-ttu-id="906f1-104">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="906f1-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="906f1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="906f1-105">Properties</span></span>
| <span data-ttu-id="906f1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="906f1-106">Property</span></span>     | <span data-ttu-id="906f1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="906f1-107">Type</span></span>   |<span data-ttu-id="906f1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="906f1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="906f1-109">number</span><span class="sxs-lookup"><span data-stu-id="906f1-109">number</span></span>|<span data-ttu-id="906f1-110">string</span><span class="sxs-lookup"><span data-stu-id="906f1-110">string</span></span>|<span data-ttu-id="906f1-111">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="906f1-111">The phone number.</span></span>|
|<span data-ttu-id="906f1-112">type</span><span class="sxs-lookup"><span data-stu-id="906f1-112">type</span></span>|<span data-ttu-id="906f1-113">PhoneType</span><span class="sxs-lookup"><span data-stu-id="906f1-113">phoneType</span></span>|<span data-ttu-id="906f1-114">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="906f1-114">The type of phone number.</span></span> <span data-ttu-id="906f1-115">Os valores possíveis são `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="906f1-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="906f1-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="906f1-116">JSON representation</span></span>

<span data-ttu-id="906f1-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="906f1-117">Here is a JSON representation of the resource.</span></span>

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
