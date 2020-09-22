---
title: tipo de recurso resultInfo
description: Isso contém informações específicas sobre o resultado de êxito e falha.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 67508afcae81fe85326eb08a4cccb69b7ef440fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991884"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="16946-103">tipo de recurso resultInfo</span><span class="sxs-lookup"><span data-stu-id="16946-103">resultInfo resource type</span></span>

<span data-ttu-id="16946-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16946-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16946-105">Isso contém informações específicas sobre o resultado de êxito e falha.</span><span class="sxs-lookup"><span data-stu-id="16946-105">This contains success and failure specific result information.</span></span> 

<span data-ttu-id="16946-106">O código especifica se o resultado é um êxito ou uma falha genérica.</span><span class="sxs-lookup"><span data-stu-id="16946-106">The code specifies if the result is a generic success or failure.</span></span> <span data-ttu-id="16946-107">Se o código for 2xx, ele será um sucesso, se for um 4xx um erro de cliente e, se for 5xx, é um erro de servidor.</span><span class="sxs-lookup"><span data-stu-id="16946-107">If the code is 2xx it's a success, if it's a 4xx it's a client error, and if it's 5xx, it's a server error.</span></span>

<span data-ttu-id="16946-108">Os subcódigos fornecem informações complementares relacionadas ao tipo de êxito ou falha (por exemplo, uma transferência de chamada foi bem-sucedida)</span><span class="sxs-lookup"><span data-stu-id="16946-108">The sub-codes provide supplementary information related to the type of success or failure (e.g. a call transfer was successful)</span></span>


## <a name="properties"></a><span data-ttu-id="16946-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16946-109">Properties</span></span>

| <span data-ttu-id="16946-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16946-110">Property</span></span> | <span data-ttu-id="16946-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="16946-111">Type</span></span>   | <span data-ttu-id="16946-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="16946-112">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="16946-113">código</span><span class="sxs-lookup"><span data-stu-id="16946-113">code</span></span>     | <span data-ttu-id="16946-114">Int32</span><span class="sxs-lookup"><span data-stu-id="16946-114">Int32</span></span> | <span data-ttu-id="16946-115">O código de resultado.</span><span class="sxs-lookup"><span data-stu-id="16946-115">The result code.</span></span>     |
| <span data-ttu-id="16946-116">mensagem</span><span class="sxs-lookup"><span data-stu-id="16946-116">message</span></span>  | <span data-ttu-id="16946-117">String</span><span class="sxs-lookup"><span data-stu-id="16946-117">String</span></span> | <span data-ttu-id="16946-118">A mensagem.</span><span class="sxs-lookup"><span data-stu-id="16946-118">The message.</span></span>         |
| <span data-ttu-id="16946-119">subcódigo</span><span class="sxs-lookup"><span data-stu-id="16946-119">subcode</span></span>  | <span data-ttu-id="16946-120">Int32</span><span class="sxs-lookup"><span data-stu-id="16946-120">Int32</span></span> | <span data-ttu-id="16946-121">O subcódigo do resultado.</span><span class="sxs-lookup"><span data-stu-id="16946-121">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16946-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16946-122">JSON representation</span></span>

<span data-ttu-id="16946-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16946-123">The following is a JSON representation of the resource.</span></span>

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

