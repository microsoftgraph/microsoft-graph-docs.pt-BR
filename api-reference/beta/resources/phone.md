---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
ms.openlocfilehash: 643b146f95fcc85be530ce7907c872f56033240e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344946"
---
# <a name="phone-resource-type"></a><span data-ttu-id="4e740-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="4e740-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e740-104">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="4e740-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="4e740-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e740-105">Properties</span></span>
| <span data-ttu-id="4e740-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e740-106">Property</span></span>     | <span data-ttu-id="4e740-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e740-107">Type</span></span>   |<span data-ttu-id="4e740-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e740-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e740-109">number</span><span class="sxs-lookup"><span data-stu-id="4e740-109">number</span></span>|<span data-ttu-id="4e740-110">string</span><span class="sxs-lookup"><span data-stu-id="4e740-110">string</span></span>|<span data-ttu-id="4e740-111">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="4e740-111">The phone number.</span></span>|
|<span data-ttu-id="4e740-112">type</span><span class="sxs-lookup"><span data-stu-id="4e740-112">type</span></span>|<span data-ttu-id="4e740-113">String</span><span class="sxs-lookup"><span data-stu-id="4e740-113">String</span></span>|<span data-ttu-id="4e740-114">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="4e740-114">The type of phone number.</span></span> <span data-ttu-id="4e740-115">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="4e740-115">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e740-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e740-116">JSON representation</span></span>

<span data-ttu-id="4e740-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e740-117">Here is a JSON representation of the resource.</span></span>

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
