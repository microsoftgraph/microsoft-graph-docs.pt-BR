---
title: Tipo de recurso CancelMediaProcessingOperation
description: Esse tipo de recurso é usado para descrever o formato de resposta da operação de cancelamento do processamento de mídia.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b1f74ba825bdd953803c3458882cbae051fae970
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042713"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="0382f-103">Tipo de recurso CancelMediaProcessingOperation</span><span class="sxs-lookup"><span data-stu-id="0382f-103">CancelMediaProcessingOperation resource type</span></span>

<span data-ttu-id="0382f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0382f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0382f-105">Descreve o formato de resposta da operação de cancelamento do processamento de mídia.</span><span class="sxs-lookup"><span data-stu-id="0382f-105">Describes the response format of media processing cancel operation.</span></span>

## <a name="properties"></a><span data-ttu-id="0382f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0382f-106">Properties</span></span>

| <span data-ttu-id="0382f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0382f-107">Property</span></span>                       | <span data-ttu-id="0382f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0382f-108">Type</span></span>                        | <span data-ttu-id="0382f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0382f-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0382f-110">todos os</span><span class="sxs-lookup"><span data-stu-id="0382f-110">all</span></span>                            | <span data-ttu-id="0382f-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="0382f-111">Boolean</span></span>                     | <span data-ttu-id="0382f-112">Indica se todas as operações ou atuais serão interrompidas.</span><span class="sxs-lookup"><span data-stu-id="0382f-112">Indicates whether to stop all operations or current.</span></span>                                                                                    |
| <span data-ttu-id="0382f-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="0382f-113">clientContext</span></span>                  | <span data-ttu-id="0382f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0382f-114">String</span></span>                      | <span data-ttu-id="0382f-115">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="0382f-115">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="0382f-116">id</span><span class="sxs-lookup"><span data-stu-id="0382f-116">id</span></span>                             | <span data-ttu-id="0382f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0382f-117">String</span></span>                      | <span data-ttu-id="0382f-118">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="0382f-118">The server operation ID.</span></span> <span data-ttu-id="0382f-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0382f-119">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="0382f-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0382f-120">resultInfo</span></span>                     | [<span data-ttu-id="0382f-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0382f-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="0382f-122">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="0382f-122">The result information.</span></span>  <span data-ttu-id="0382f-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0382f-123">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="0382f-124">status</span><span class="sxs-lookup"><span data-stu-id="0382f-124">status</span></span>                         | <span data-ttu-id="0382f-125">String</span><span class="sxs-lookup"><span data-stu-id="0382f-125">String</span></span>                      | <span data-ttu-id="0382f-126">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0382f-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="0382f-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0382f-127">Read-only.</span></span>                                                  |

## <a name="relationships"></a><span data-ttu-id="0382f-128">Relações</span><span class="sxs-lookup"><span data-stu-id="0382f-128">Relationships</span></span>
<span data-ttu-id="0382f-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0382f-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0382f-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0382f-130">JSON representation</span></span>

<span data-ttu-id="0382f-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0382f-131">The following is a JSON representation of the resource.</span></span>

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


