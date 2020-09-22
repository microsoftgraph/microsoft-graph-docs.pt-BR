---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: davidmu1
ms.openlocfilehash: 0e87557a3c31ef1fb8f5ebbbdd2ff29b67d8ff8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997897"
---
# <a name="phone-resource-type"></a><span data-ttu-id="15633-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="15633-103">phone resource type</span></span>

<span data-ttu-id="15633-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15633-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15633-105">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="15633-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="15633-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15633-106">Properties</span></span>
| <span data-ttu-id="15633-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15633-107">Property</span></span>     | <span data-ttu-id="15633-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="15633-108">Type</span></span>   |<span data-ttu-id="15633-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="15633-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15633-110">number</span><span class="sxs-lookup"><span data-stu-id="15633-110">number</span></span>|<span data-ttu-id="15633-111">string</span><span class="sxs-lookup"><span data-stu-id="15633-111">string</span></span>|<span data-ttu-id="15633-112">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="15633-112">The phone number.</span></span>|
|<span data-ttu-id="15633-113">tipo</span><span class="sxs-lookup"><span data-stu-id="15633-113">type</span></span>|<span data-ttu-id="15633-114">String</span><span class="sxs-lookup"><span data-stu-id="15633-114">String</span></span>|<span data-ttu-id="15633-115">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="15633-115">The type of phone number.</span></span> <span data-ttu-id="15633-116">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="15633-116">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15633-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15633-117">JSON representation</span></span>

<span data-ttu-id="15633-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15633-118">Here is a JSON representation of the resource.</span></span>

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


