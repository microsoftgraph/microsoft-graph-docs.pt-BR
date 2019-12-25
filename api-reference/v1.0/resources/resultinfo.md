---
title: tipo de recurso resultInfo
description: Isso contém informações específicas sobre o resultado de êxito e falha.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 39027ecf949860d9ffa757a95839ae7fd8184a27
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865644"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="d4f72-103">tipo de recurso resultInfo</span><span class="sxs-lookup"><span data-stu-id="d4f72-103">resultInfo resource type</span></span>

<span data-ttu-id="d4f72-104">Isso contém informações específicas sobre o resultado de êxito e falha.</span><span class="sxs-lookup"><span data-stu-id="d4f72-104">This contains success and failure specific result information.</span></span> 

<span data-ttu-id="d4f72-105">O código especifica se o resultado é um êxito ou uma falha genérica.</span><span class="sxs-lookup"><span data-stu-id="d4f72-105">The code specifies if the result is a generic success or failure.</span></span> <span data-ttu-id="d4f72-106">Se o código for 2xx, ele será um sucesso, se for um 4xx um erro de cliente e, se for 5xx, é um erro de servidor.</span><span class="sxs-lookup"><span data-stu-id="d4f72-106">If the code is 2xx it's a success, if it's a 4xx it's a client error, and if it's 5xx, it's a server error.</span></span>

<span data-ttu-id="d4f72-107">Os subcódigos fornecem informações complementares relacionadas ao tipo de êxito ou falha (por exemplo, uma transferência de chamada foi bem-sucedida)</span><span class="sxs-lookup"><span data-stu-id="d4f72-107">The sub-codes provide supplementary information related to the type of success or failure (e.g. a call transfer was successful)</span></span>


## <a name="properties"></a><span data-ttu-id="d4f72-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4f72-108">Properties</span></span>

| <span data-ttu-id="d4f72-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4f72-109">Property</span></span> | <span data-ttu-id="d4f72-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4f72-110">Type</span></span>   | <span data-ttu-id="d4f72-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4f72-111">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="d4f72-112">código</span><span class="sxs-lookup"><span data-stu-id="d4f72-112">code</span></span>     | <span data-ttu-id="d4f72-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d4f72-113">Int32</span></span> | <span data-ttu-id="d4f72-114">O código de resultado.</span><span class="sxs-lookup"><span data-stu-id="d4f72-114">The result code.</span></span>     |
| <span data-ttu-id="d4f72-115">mensagem</span><span class="sxs-lookup"><span data-stu-id="d4f72-115">message</span></span>  | <span data-ttu-id="d4f72-116">String</span><span class="sxs-lookup"><span data-stu-id="d4f72-116">String</span></span> | <span data-ttu-id="d4f72-117">A mensagem.</span><span class="sxs-lookup"><span data-stu-id="d4f72-117">The message.</span></span>         |
| <span data-ttu-id="d4f72-118">subcódigo</span><span class="sxs-lookup"><span data-stu-id="d4f72-118">subcode</span></span>  | <span data-ttu-id="d4f72-119">Int32</span><span class="sxs-lookup"><span data-stu-id="d4f72-119">Int32</span></span> | <span data-ttu-id="d4f72-120">O subcódigo do resultado.</span><span class="sxs-lookup"><span data-stu-id="d4f72-120">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4f72-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4f72-121">JSON representation</span></span>

<span data-ttu-id="d4f72-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4f72-122">The following is a JSON representation of the resource.</span></span>

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
