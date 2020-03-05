---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2e20932285f7009ee470ba66a6a9cd78c50d65ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447182"
---
# <a name="phone-resource-type"></a><span data-ttu-id="378d3-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="378d3-103">phone resource type</span></span>

<span data-ttu-id="378d3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="378d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="378d3-105">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="378d3-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="378d3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="378d3-106">Properties</span></span>
| <span data-ttu-id="378d3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="378d3-107">Property</span></span>     | <span data-ttu-id="378d3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="378d3-108">Type</span></span>   |<span data-ttu-id="378d3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="378d3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="378d3-110">number</span><span class="sxs-lookup"><span data-stu-id="378d3-110">number</span></span>|<span data-ttu-id="378d3-111">string</span><span class="sxs-lookup"><span data-stu-id="378d3-111">string</span></span>|<span data-ttu-id="378d3-112">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="378d3-112">The phone number.</span></span>|
|<span data-ttu-id="378d3-113">type</span><span class="sxs-lookup"><span data-stu-id="378d3-113">type</span></span>|<span data-ttu-id="378d3-114">PhoneType</span><span class="sxs-lookup"><span data-stu-id="378d3-114">phoneType</span></span>|<span data-ttu-id="378d3-115">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="378d3-115">The type of phone number.</span></span> <span data-ttu-id="378d3-116">Os valores possíveis são `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="378d3-116">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="378d3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="378d3-117">JSON representation</span></span>

<span data-ttu-id="378d3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="378d3-118">Here is a JSON representation of the resource.</span></span>

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
