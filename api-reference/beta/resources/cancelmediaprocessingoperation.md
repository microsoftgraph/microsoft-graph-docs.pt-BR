---
title: Tipo de recurso CancelMediaProcessingOperation
description: Esse tipo de recurso é usado para descrever o formato de resposta da operação de cancelamento do processamento de mídia.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 700c63b2b620117f25df876544aeb6fb0e6d0230
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507779"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="9e82c-103">Tipo de recurso CancelMediaProcessingOperation</span><span class="sxs-lookup"><span data-stu-id="9e82c-103">CancelMediaProcessingOperation resource type</span></span>

<span data-ttu-id="9e82c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9e82c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e82c-105">Descreve o formato de resposta da operação de cancelamento do processamento de mídia.</span><span class="sxs-lookup"><span data-stu-id="9e82c-105">Describes the response format of media processing cancel operation.</span></span>

## <a name="properties"></a><span data-ttu-id="9e82c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e82c-106">Properties</span></span>

| <span data-ttu-id="9e82c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e82c-107">Property</span></span>                       | <span data-ttu-id="9e82c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e82c-108">Type</span></span>                        | <span data-ttu-id="9e82c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e82c-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9e82c-110">todos os</span><span class="sxs-lookup"><span data-stu-id="9e82c-110">all</span></span>                            | <span data-ttu-id="9e82c-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e82c-111">Boolean</span></span>                     | <span data-ttu-id="9e82c-112">Indica se todas as operações ou atuais serão interrompidas.</span><span class="sxs-lookup"><span data-stu-id="9e82c-112">Indicates whether to stop all operations or current.</span></span>                                                                                    |
| <span data-ttu-id="9e82c-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="9e82c-113">clientContext</span></span>                  | <span data-ttu-id="9e82c-114">String</span><span class="sxs-lookup"><span data-stu-id="9e82c-114">String</span></span>                      | <span data-ttu-id="9e82c-115">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="9e82c-115">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="9e82c-116">id</span><span class="sxs-lookup"><span data-stu-id="9e82c-116">id</span></span>                             | <span data-ttu-id="9e82c-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e82c-117">String</span></span>                      | <span data-ttu-id="9e82c-118">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="9e82c-118">The server operation ID.</span></span> <span data-ttu-id="9e82c-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e82c-119">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="9e82c-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9e82c-120">resultInfo</span></span>                     | [<span data-ttu-id="9e82c-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9e82c-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="9e82c-122">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="9e82c-122">The result information.</span></span>  <span data-ttu-id="9e82c-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e82c-123">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="9e82c-124">status</span><span class="sxs-lookup"><span data-stu-id="9e82c-124">status</span></span>                         | <span data-ttu-id="9e82c-125">String</span><span class="sxs-lookup"><span data-stu-id="9e82c-125">String</span></span>                      | <span data-ttu-id="9e82c-126">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9e82c-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="9e82c-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e82c-127">Read-only.</span></span>                                                  |

## <a name="relationships"></a><span data-ttu-id="9e82c-128">Relações</span><span class="sxs-lookup"><span data-stu-id="9e82c-128">Relationships</span></span>
<span data-ttu-id="9e82c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e82c-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e82c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e82c-130">JSON representation</span></span>

<span data-ttu-id="9e82c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e82c-131">The following is a JSON representation of the resource.</span></span>

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
