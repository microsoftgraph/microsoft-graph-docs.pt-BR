---
title: tipo de recurso cancelMediaProcessingOperation
description: Esse tipo de recurso é usado para descrever o formato de resposta da operação de processamento de mídia de cancelamento.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5962b3f5aed89c7f2c0b01be3f8b4a035ac463da
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319602"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="cc2aa-103">Tipo de recurso CancelMediaProcessingOperation</span><span class="sxs-lookup"><span data-stu-id="cc2aa-103">CancelMediaProcessingOperation resource type</span></span>

<span data-ttu-id="cc2aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc2aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc2aa-105">Descreve o formato de resposta da operação de processamento de mídia de cancelamento.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-105">Describes the response format of the cancel media processing operation.</span></span>

## <a name="properties"></a><span data-ttu-id="cc2aa-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc2aa-106">Properties</span></span>

| <span data-ttu-id="cc2aa-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc2aa-107">Property</span></span>      | <span data-ttu-id="cc2aa-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc2aa-108">Type</span></span>                        | <span data-ttu-id="cc2aa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc2aa-109">Description</span></span>                                                                     |
| :------------ | :-------------------------- | :------------------------------------------------------------------------------ |
| <span data-ttu-id="cc2aa-110">todos os</span><span class="sxs-lookup"><span data-stu-id="cc2aa-110">all</span></span>           | <span data-ttu-id="cc2aa-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="cc2aa-111">Boolean</span></span>                     | <span data-ttu-id="cc2aa-112">Indica se todas as operações ou atuais serão interrompidas.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-112">Indicates whether to stop all operations or current.</span></span>                            |
| <span data-ttu-id="cc2aa-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="cc2aa-113">clientContext</span></span> | <span data-ttu-id="cc2aa-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc2aa-114">String</span></span>                      | <span data-ttu-id="cc2aa-115">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-115">The client context.</span></span>                                                             |
| <span data-ttu-id="cc2aa-116">id</span><span class="sxs-lookup"><span data-stu-id="cc2aa-116">id</span></span>            | <span data-ttu-id="cc2aa-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc2aa-117">String</span></span>                      | <span data-ttu-id="cc2aa-118">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-118">The server operation ID.</span></span> <span data-ttu-id="cc2aa-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-119">Read-only.</span></span>                                             |
| <span data-ttu-id="cc2aa-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cc2aa-120">resultInfo</span></span>    | [<span data-ttu-id="cc2aa-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cc2aa-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="cc2aa-122">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-122">The result information.</span></span>  <span data-ttu-id="cc2aa-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-123">Read-only.</span></span>                                             |
| <span data-ttu-id="cc2aa-124">status</span><span class="sxs-lookup"><span data-stu-id="cc2aa-124">status</span></span>        | <span data-ttu-id="cc2aa-125">String</span><span class="sxs-lookup"><span data-stu-id="cc2aa-125">String</span></span>                      | <span data-ttu-id="cc2aa-126">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="cc2aa-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-127">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cc2aa-128">Relações</span><span class="sxs-lookup"><span data-stu-id="cc2aa-128">Relationships</span></span>
<span data-ttu-id="cc2aa-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc2aa-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc2aa-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc2aa-130">JSON representation</span></span>

<span data-ttu-id="cc2aa-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc2aa-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
}-->
```json
{
  "all": true,
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cancelMediaProcessingOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
