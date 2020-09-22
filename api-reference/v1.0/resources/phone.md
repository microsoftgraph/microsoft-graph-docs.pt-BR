---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a5b62fd10a26f06e983a98937e0d434674330767
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022831"
---
# <a name="phone-resource-type"></a><span data-ttu-id="c0fc8-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="c0fc8-103">phone resource type</span></span>

<span data-ttu-id="c0fc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0fc8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0fc8-105">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c0fc8-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="c0fc8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0fc8-106">Properties</span></span>
| <span data-ttu-id="c0fc8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0fc8-107">Property</span></span>     | <span data-ttu-id="c0fc8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0fc8-108">Type</span></span>   |<span data-ttu-id="c0fc8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0fc8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0fc8-110">number</span><span class="sxs-lookup"><span data-stu-id="c0fc8-110">number</span></span>|<span data-ttu-id="c0fc8-111">string</span><span class="sxs-lookup"><span data-stu-id="c0fc8-111">string</span></span>|<span data-ttu-id="c0fc8-112">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c0fc8-112">The phone number.</span></span>|
|<span data-ttu-id="c0fc8-113">tipo</span><span class="sxs-lookup"><span data-stu-id="c0fc8-113">type</span></span>|<span data-ttu-id="c0fc8-114">PhoneType</span><span class="sxs-lookup"><span data-stu-id="c0fc8-114">phoneType</span></span>|<span data-ttu-id="c0fc8-115">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c0fc8-115">The type of phone number.</span></span> <span data-ttu-id="c0fc8-116">Os valores possíveis são `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="c0fc8-116">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0fc8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0fc8-117">JSON representation</span></span>

<span data-ttu-id="c0fc8-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0fc8-118">Here is a JSON representation of the resource.</span></span>

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

