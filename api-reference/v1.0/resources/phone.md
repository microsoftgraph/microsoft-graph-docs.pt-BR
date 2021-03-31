---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6740d1cd1746151d35f7627d9ab5125724adc3f0
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469231"
---
# <a name="phone-resource-type"></a><span data-ttu-id="efba3-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="efba3-103">phone resource type</span></span>

<span data-ttu-id="efba3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efba3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efba3-105">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="efba3-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="efba3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efba3-106">Properties</span></span>
| <span data-ttu-id="efba3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efba3-107">Property</span></span>     | <span data-ttu-id="efba3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="efba3-108">Type</span></span>   |<span data-ttu-id="efba3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="efba3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efba3-110">number</span><span class="sxs-lookup"><span data-stu-id="efba3-110">number</span></span>|<span data-ttu-id="efba3-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efba3-111">string</span></span>|<span data-ttu-id="efba3-112">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="efba3-112">The phone number.</span></span>|
|<span data-ttu-id="efba3-113">tipo</span><span class="sxs-lookup"><span data-stu-id="efba3-113">type</span></span>|<span data-ttu-id="efba3-114">phoneType</span><span class="sxs-lookup"><span data-stu-id="efba3-114">phoneType</span></span>|<span data-ttu-id="efba3-115">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="efba3-115">The type of phone number.</span></span> <span data-ttu-id="efba3-116">Os valores possíveis são `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="efba3-116">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efba3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efba3-117">JSON representation</span></span>

<span data-ttu-id="efba3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efba3-118">Here is a JSON representation of the resource.</span></span>

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

