---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ad7438e532420d15f14096a0843b42456a4b1fbc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966110"
---
# <a name="phone-resource-type"></a><span data-ttu-id="c3025-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="c3025-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3025-104">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c3025-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="c3025-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3025-105">Properties</span></span>
| <span data-ttu-id="c3025-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3025-106">Property</span></span>     | <span data-ttu-id="c3025-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3025-107">Type</span></span>   |<span data-ttu-id="c3025-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3025-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3025-109">number</span><span class="sxs-lookup"><span data-stu-id="c3025-109">number</span></span>|<span data-ttu-id="c3025-110">string</span><span class="sxs-lookup"><span data-stu-id="c3025-110">string</span></span>|<span data-ttu-id="c3025-111">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c3025-111">The phone number.</span></span>|
|<span data-ttu-id="c3025-112">type</span><span class="sxs-lookup"><span data-stu-id="c3025-112">type</span></span>|<span data-ttu-id="c3025-113">String</span><span class="sxs-lookup"><span data-stu-id="c3025-113">String</span></span>|<span data-ttu-id="c3025-114">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c3025-114">The type of phone number.</span></span> <span data-ttu-id="c3025-115">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="c3025-115">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3025-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3025-116">JSON representation</span></span>

<span data-ttu-id="c3025-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3025-117">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
