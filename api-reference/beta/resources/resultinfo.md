---
title: tipo de recurso resultInfo
description: Contém informações de resultado específicas de êxito e falha.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa55f8cdcb7ca4639aa4975a28ae2bcbcd625588
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521079"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="0262e-103">tipo de recurso resultInfo</span><span class="sxs-lookup"><span data-stu-id="0262e-103">resultInfo resource type</span></span>

<span data-ttu-id="0262e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0262e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0262e-105">Contém informações de resultado específicas de êxito e falha.</span><span class="sxs-lookup"><span data-stu-id="0262e-105">Contains success and failure-specific result information.</span></span> 

<span data-ttu-id="0262e-106">O código especifica se o resultado é um êxito ou uma falha genérica.</span><span class="sxs-lookup"><span data-stu-id="0262e-106">The code specifies whether the result is a generic success or failure.</span></span> 

<span data-ttu-id="0262e-107">Os subcódigos fornecem informações complementares relacionadas ao tipo de sucesso ou falha (por exemplo, uma transferência de chamada foi bem-sucedida).</span><span class="sxs-lookup"><span data-stu-id="0262e-107">The subcodes provide supplementary information related to the type of success or failure (for example, a call transfer was successful).</span></span>


## <a name="properties"></a><span data-ttu-id="0262e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0262e-108">Properties</span></span>

| <span data-ttu-id="0262e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0262e-109">Property</span></span> | <span data-ttu-id="0262e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0262e-110">Type</span></span>   | <span data-ttu-id="0262e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0262e-111">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="0262e-112">código</span><span class="sxs-lookup"><span data-stu-id="0262e-112">code</span></span>     | <span data-ttu-id="0262e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0262e-113">Int32</span></span> | <span data-ttu-id="0262e-114">O código de resultado.</span><span class="sxs-lookup"><span data-stu-id="0262e-114">The result code.</span></span>     |
| <span data-ttu-id="0262e-115">mensagem</span><span class="sxs-lookup"><span data-stu-id="0262e-115">message</span></span>  | <span data-ttu-id="0262e-116">String</span><span class="sxs-lookup"><span data-stu-id="0262e-116">String</span></span> | <span data-ttu-id="0262e-117">A mensagem.</span><span class="sxs-lookup"><span data-stu-id="0262e-117">The message.</span></span>         |
| <span data-ttu-id="0262e-118">subcódigo</span><span class="sxs-lookup"><span data-stu-id="0262e-118">subcode</span></span>  | <span data-ttu-id="0262e-119">Int32</span><span class="sxs-lookup"><span data-stu-id="0262e-119">Int32</span></span> | <span data-ttu-id="0262e-120">O subcódigo do resultado.</span><span class="sxs-lookup"><span data-stu-id="0262e-120">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0262e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0262e-121">JSON representation</span></span>

<span data-ttu-id="0262e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0262e-122">The following is a JSON representation of the resource.</span></span>

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
