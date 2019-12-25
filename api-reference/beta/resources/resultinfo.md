---
title: tipo de recurso resultInfo
description: Contém informações de resultado específicas de êxito e falha.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5cb59cb63ff7c50ba14b972991d54806eabc4f54
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866627"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="6117a-103">tipo de recurso resultInfo</span><span class="sxs-lookup"><span data-stu-id="6117a-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6117a-104">Contém informações de resultado específicas de êxito e falha.</span><span class="sxs-lookup"><span data-stu-id="6117a-104">Contains success and failure-specific result information.</span></span> 

<span data-ttu-id="6117a-105">O código especifica se o resultado é um êxito ou uma falha genérica.</span><span class="sxs-lookup"><span data-stu-id="6117a-105">The code specifies whether the result is a generic success or failure.</span></span> 

<span data-ttu-id="6117a-106">Os subcódigos fornecem informações complementares relacionadas ao tipo de sucesso ou falha (por exemplo, uma transferência de chamada foi bem-sucedida).</span><span class="sxs-lookup"><span data-stu-id="6117a-106">The subcodes provide supplementary information related to the type of success or failure (for example, a call transfer was successful).</span></span>


## <a name="properties"></a><span data-ttu-id="6117a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6117a-107">Properties</span></span>

| <span data-ttu-id="6117a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6117a-108">Property</span></span> | <span data-ttu-id="6117a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6117a-109">Type</span></span>   | <span data-ttu-id="6117a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6117a-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="6117a-111">código</span><span class="sxs-lookup"><span data-stu-id="6117a-111">code</span></span>     | <span data-ttu-id="6117a-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6117a-112">Int32</span></span> | <span data-ttu-id="6117a-113">O código de resultado.</span><span class="sxs-lookup"><span data-stu-id="6117a-113">The result code.</span></span>     |
| <span data-ttu-id="6117a-114">mensagem</span><span class="sxs-lookup"><span data-stu-id="6117a-114">message</span></span>  | <span data-ttu-id="6117a-115">String</span><span class="sxs-lookup"><span data-stu-id="6117a-115">String</span></span> | <span data-ttu-id="6117a-116">A mensagem.</span><span class="sxs-lookup"><span data-stu-id="6117a-116">The message.</span></span>         |
| <span data-ttu-id="6117a-117">subcódigo</span><span class="sxs-lookup"><span data-stu-id="6117a-117">subcode</span></span>  | <span data-ttu-id="6117a-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6117a-118">Int32</span></span> | <span data-ttu-id="6117a-119">O subcódigo do resultado.</span><span class="sxs-lookup"><span data-stu-id="6117a-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6117a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6117a-120">JSON representation</span></span>

<span data-ttu-id="6117a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6117a-121">The following is a JSON representation of the resource.</span></span>

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
