---
title: Tipo de recurso CancelMediaProcessingOperation
description: Esse tipo de recurso é usado para descrever o formato de resposta da operação de cancelamento do processamento de mídia.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20da55c068f6e0f0a69b876cfd23181eac1391a4
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913496"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="4baf9-103">Tipo de recurso CancelMediaProcessingOperation</span><span class="sxs-lookup"><span data-stu-id="4baf9-103">CancelMediaProcessingOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4baf9-104">Descreve o formato de resposta da operação de cancelamento do processamento de mídia.</span><span class="sxs-lookup"><span data-stu-id="4baf9-104">Describes the response format of media processing cancel operation.</span></span>

## <a name="properties"></a><span data-ttu-id="4baf9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4baf9-105">Properties</span></span>

| <span data-ttu-id="4baf9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4baf9-106">Property</span></span>                       | <span data-ttu-id="4baf9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4baf9-107">Type</span></span>                        | <span data-ttu-id="4baf9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4baf9-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4baf9-109">todos os</span><span class="sxs-lookup"><span data-stu-id="4baf9-109">all</span></span>                            | <span data-ttu-id="4baf9-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="4baf9-110">Boolean</span></span>                     | <span data-ttu-id="4baf9-111">Indica se todas as operações ou atuais serão interrompidas.</span><span class="sxs-lookup"><span data-stu-id="4baf9-111">Indicates whether to stop all operations or current.</span></span>                                                                                    |
| <span data-ttu-id="4baf9-112">clientContext</span><span class="sxs-lookup"><span data-stu-id="4baf9-112">clientContext</span></span>                  | <span data-ttu-id="4baf9-113">String</span><span class="sxs-lookup"><span data-stu-id="4baf9-113">String</span></span>                      | <span data-ttu-id="4baf9-114">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="4baf9-114">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="4baf9-115">id</span><span class="sxs-lookup"><span data-stu-id="4baf9-115">id</span></span>                             | <span data-ttu-id="4baf9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4baf9-116">String</span></span>                      | <span data-ttu-id="4baf9-117">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="4baf9-117">The server operation ID.</span></span> <span data-ttu-id="4baf9-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4baf9-118">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="4baf9-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4baf9-119">resultInfo</span></span>                     | [<span data-ttu-id="4baf9-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4baf9-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="4baf9-121">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="4baf9-121">The result information.</span></span>  <span data-ttu-id="4baf9-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4baf9-122">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="4baf9-123">status</span><span class="sxs-lookup"><span data-stu-id="4baf9-123">status</span></span>                         | <span data-ttu-id="4baf9-124">String</span><span class="sxs-lookup"><span data-stu-id="4baf9-124">String</span></span>                      | <span data-ttu-id="4baf9-125">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="4baf9-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="4baf9-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4baf9-126">Read-only.</span></span>                                                  |

## <a name="relationships"></a><span data-ttu-id="4baf9-127">Relações</span><span class="sxs-lookup"><span data-stu-id="4baf9-127">Relationships</span></span>
<span data-ttu-id="4baf9-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4baf9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4baf9-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4baf9-129">JSON representation</span></span>

<span data-ttu-id="4baf9-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4baf9-130">The following is a JSON representation of the resource.</span></span>

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
