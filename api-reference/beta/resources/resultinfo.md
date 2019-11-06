---
title: tipo de recurso resultInfo
description: O tipo resultInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: acc01a17420390343c3eb1f866761d54d5c81c79
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006547"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="fb29c-103">tipo de recurso resultInfo</span><span class="sxs-lookup"><span data-stu-id="fb29c-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb29c-104">O tipo resultInfo.</span><span class="sxs-lookup"><span data-stu-id="fb29c-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="fb29c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb29c-105">Properties</span></span>

| <span data-ttu-id="fb29c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb29c-106">Property</span></span> | <span data-ttu-id="fb29c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb29c-107">Type</span></span>   | <span data-ttu-id="fb29c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb29c-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="fb29c-109">código</span><span class="sxs-lookup"><span data-stu-id="fb29c-109">code</span></span>     | <span data-ttu-id="fb29c-110">Int32</span><span class="sxs-lookup"><span data-stu-id="fb29c-110">Int32</span></span> | <span data-ttu-id="fb29c-111">O código de resultado.</span><span class="sxs-lookup"><span data-stu-id="fb29c-111">The result code.</span></span>     |
| <span data-ttu-id="fb29c-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="fb29c-112">message</span></span>  | <span data-ttu-id="fb29c-113">String</span><span class="sxs-lookup"><span data-stu-id="fb29c-113">String</span></span> | <span data-ttu-id="fb29c-114">A mensagem.</span><span class="sxs-lookup"><span data-stu-id="fb29c-114">The message.</span></span>         |
| <span data-ttu-id="fb29c-115">subcódigo</span><span class="sxs-lookup"><span data-stu-id="fb29c-115">subcode</span></span>  | <span data-ttu-id="fb29c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fb29c-116">Int32</span></span> | <span data-ttu-id="fb29c-117">O subcódigo do resultado.</span><span class="sxs-lookup"><span data-stu-id="fb29c-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fb29c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb29c-118">JSON representation</span></span>

<span data-ttu-id="fb29c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb29c-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": 0,
  "message": "String",
  "subcode": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
