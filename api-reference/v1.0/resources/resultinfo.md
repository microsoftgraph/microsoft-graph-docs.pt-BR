---
title: tipo de recurso resultInfo
description: Isso contém informações específicas sobre o resultado de êxito e falha.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42b636b09e8cfeb2ed41578e06fc57b5aa976fd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533818"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="889b0-103">tipo de recurso resultInfo</span><span class="sxs-lookup"><span data-stu-id="889b0-103">resultInfo resource type</span></span>

<span data-ttu-id="889b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="889b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="889b0-105">Isso contém informações específicas sobre o resultado de êxito e falha.</span><span class="sxs-lookup"><span data-stu-id="889b0-105">This contains success and failure specific result information.</span></span> 

<span data-ttu-id="889b0-106">O código especifica se o resultado é um êxito ou uma falha genérica.</span><span class="sxs-lookup"><span data-stu-id="889b0-106">The code specifies if the result is a generic success or failure.</span></span> <span data-ttu-id="889b0-107">Se o código for 2xx, ele será um sucesso, se for um 4xx um erro de cliente e, se for 5xx, é um erro de servidor.</span><span class="sxs-lookup"><span data-stu-id="889b0-107">If the code is 2xx it's a success, if it's a 4xx it's a client error, and if it's 5xx, it's a server error.</span></span>

<span data-ttu-id="889b0-108">Os subcódigos fornecem informações complementares relacionadas ao tipo de êxito ou falha (por exemplo, uma transferência de chamada foi bem-sucedida)</span><span class="sxs-lookup"><span data-stu-id="889b0-108">The sub-codes provide supplementary information related to the type of success or failure (e.g. a call transfer was successful)</span></span>


## <a name="properties"></a><span data-ttu-id="889b0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="889b0-109">Properties</span></span>

| <span data-ttu-id="889b0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="889b0-110">Property</span></span> | <span data-ttu-id="889b0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="889b0-111">Type</span></span>   | <span data-ttu-id="889b0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="889b0-112">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="889b0-113">código</span><span class="sxs-lookup"><span data-stu-id="889b0-113">code</span></span>     | <span data-ttu-id="889b0-114">Int32</span><span class="sxs-lookup"><span data-stu-id="889b0-114">Int32</span></span> | <span data-ttu-id="889b0-115">O código de resultado.</span><span class="sxs-lookup"><span data-stu-id="889b0-115">The result code.</span></span>     |
| <span data-ttu-id="889b0-116">mensagem</span><span class="sxs-lookup"><span data-stu-id="889b0-116">message</span></span>  | <span data-ttu-id="889b0-117">String</span><span class="sxs-lookup"><span data-stu-id="889b0-117">String</span></span> | <span data-ttu-id="889b0-118">A mensagem.</span><span class="sxs-lookup"><span data-stu-id="889b0-118">The message.</span></span>         |
| <span data-ttu-id="889b0-119">subcódigo</span><span class="sxs-lookup"><span data-stu-id="889b0-119">subcode</span></span>  | <span data-ttu-id="889b0-120">Int32</span><span class="sxs-lookup"><span data-stu-id="889b0-120">Int32</span></span> | <span data-ttu-id="889b0-121">O subcódigo do resultado.</span><span class="sxs-lookup"><span data-stu-id="889b0-121">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="889b0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="889b0-122">JSON representation</span></span>

<span data-ttu-id="889b0-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="889b0-123">The following is a JSON representation of the resource.</span></span>

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
