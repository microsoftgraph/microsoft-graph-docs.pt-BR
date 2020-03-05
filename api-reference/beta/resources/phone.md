---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ca2c81531aa5bf53c8038fe7e095f056c4682eba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521887"
---
# <a name="phone-resource-type"></a><span data-ttu-id="e5d84-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="e5d84-103">phone resource type</span></span>

<span data-ttu-id="e5d84-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e5d84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5d84-105">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="e5d84-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="e5d84-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5d84-106">Properties</span></span>
| <span data-ttu-id="e5d84-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5d84-107">Property</span></span>     | <span data-ttu-id="e5d84-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5d84-108">Type</span></span>   |<span data-ttu-id="e5d84-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5d84-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5d84-110">number</span><span class="sxs-lookup"><span data-stu-id="e5d84-110">number</span></span>|<span data-ttu-id="e5d84-111">string</span><span class="sxs-lookup"><span data-stu-id="e5d84-111">string</span></span>|<span data-ttu-id="e5d84-112">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="e5d84-112">The phone number.</span></span>|
|<span data-ttu-id="e5d84-113">type</span><span class="sxs-lookup"><span data-stu-id="e5d84-113">type</span></span>|<span data-ttu-id="e5d84-114">String</span><span class="sxs-lookup"><span data-stu-id="e5d84-114">String</span></span>|<span data-ttu-id="e5d84-115">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="e5d84-115">The type of phone number.</span></span> <span data-ttu-id="e5d84-116">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="e5d84-116">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5d84-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5d84-117">JSON representation</span></span>

<span data-ttu-id="e5d84-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5d84-118">Here is a JSON representation of the resource.</span></span>

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
