---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: davidmu1
ms.openlocfilehash: 7c6ee74a588540470ceeffcc37b51e29e7e4f597
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130862"
---
# <a name="phone-resource-type"></a><span data-ttu-id="7203f-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="7203f-103">phone resource type</span></span>

<span data-ttu-id="7203f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7203f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7203f-105">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="7203f-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="7203f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7203f-106">Properties</span></span>
| <span data-ttu-id="7203f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7203f-107">Property</span></span>     | <span data-ttu-id="7203f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7203f-108">Type</span></span>   |<span data-ttu-id="7203f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7203f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7203f-110">number</span><span class="sxs-lookup"><span data-stu-id="7203f-110">number</span></span>|<span data-ttu-id="7203f-111">string</span><span class="sxs-lookup"><span data-stu-id="7203f-111">string</span></span>|<span data-ttu-id="7203f-112">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="7203f-112">The phone number.</span></span>|
|<span data-ttu-id="7203f-113">type</span><span class="sxs-lookup"><span data-stu-id="7203f-113">type</span></span>|<span data-ttu-id="7203f-114">String</span><span class="sxs-lookup"><span data-stu-id="7203f-114">String</span></span>|<span data-ttu-id="7203f-115">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="7203f-115">The type of phone number.</span></span> <span data-ttu-id="7203f-116">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="7203f-116">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7203f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7203f-117">JSON representation</span></span>

<span data-ttu-id="7203f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7203f-118">Here is a JSON representation of the resource.</span></span>

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


