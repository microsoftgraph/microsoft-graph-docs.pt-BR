---
title: tipo de recurso commsOperation
description: O status de determinadas operações de longa duração.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 664079223e9dc6fe685ad52d0112f74cb4264aab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033941"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="868c9-103">tipo de recurso commsOperation</span><span class="sxs-lookup"><span data-stu-id="868c9-103">commsOperation resource type</span></span>

<span data-ttu-id="868c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="868c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="868c9-105">Representa o status de determinadas operações de longa duração.</span><span class="sxs-lookup"><span data-stu-id="868c9-105">Represents the status of certain long-running operations.</span></span>

<span data-ttu-id="868c9-106">Esse recurso pode ser retornado como a resposta a uma ação ou como o conteúdo de um [commsNotification](commsNotification.md).</span><span class="sxs-lookup"><span data-stu-id="868c9-106">This resource can be returned as the response to an action, or as the content of a [commsNotification](commsNotification.md).</span></span>  

<span data-ttu-id="868c9-107">Quando ele é retornado como uma resposta a uma ação, o status indica se haverá notificações subsequentes.</span><span class="sxs-lookup"><span data-stu-id="868c9-107">When it is returned as a response to an action, the status indicates whether there will be subsequent notifications.</span></span> <span data-ttu-id="868c9-108">Se, por exemplo, uma operação com status `completed` ou `failed` for retornada, não haverá nenhuma operação subsequente por meio do canal de notificação.</span><span class="sxs-lookup"><span data-stu-id="868c9-108">If, for example, an operation with status of `completed` or `failed` is returned,  there will not be any subsequent operation via the notification channel.</span></span> 

<span data-ttu-id="868c9-109">Se uma `null` operação ou uma operação com o status `notStarted` ou `running` for retornada, as atualizações subsequentes serão fornecidas pelo canal de notificação.</span><span class="sxs-lookup"><span data-stu-id="868c9-109">If a `null` operation, or an operation with a status of `notStarted` or `running` is returned, subsequent updates will come via the notification channel.</span></span>

## <a name="properties"></a><span data-ttu-id="868c9-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="868c9-110">Properties</span></span>

| <span data-ttu-id="868c9-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="868c9-111">Property</span></span>           | <span data-ttu-id="868c9-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="868c9-112">Type</span></span>                        | <span data-ttu-id="868c9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="868c9-113">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="868c9-114">clientContext</span><span class="sxs-lookup"><span data-stu-id="868c9-114">clientContext</span></span>      | <span data-ttu-id="868c9-115">String</span><span class="sxs-lookup"><span data-stu-id="868c9-115">String</span></span>                      | <span data-ttu-id="868c9-116">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="868c9-116">Unique Client Context string.</span></span> <span data-ttu-id="868c9-117">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="868c9-117">Max limit is 256 chars.</span></span>                           |
| <span data-ttu-id="868c9-118">id</span><span class="sxs-lookup"><span data-stu-id="868c9-118">id</span></span>                 | <span data-ttu-id="868c9-119">String</span><span class="sxs-lookup"><span data-stu-id="868c9-119">String</span></span>                      | <span data-ttu-id="868c9-120">A ID da operação.</span><span class="sxs-lookup"><span data-stu-id="868c9-120">The operation ID.</span></span> <span data-ttu-id="868c9-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="868c9-121">Read-only.</span></span>                                                    |
| <span data-ttu-id="868c9-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="868c9-122">resultInfo</span></span>         | [<span data-ttu-id="868c9-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="868c9-123">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="868c9-124">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="868c9-124">The result information.</span></span> <span data-ttu-id="868c9-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="868c9-125">Read-only.</span></span>                                              |
| <span data-ttu-id="868c9-126">status</span><span class="sxs-lookup"><span data-stu-id="868c9-126">status</span></span>             | <span data-ttu-id="868c9-127">String</span><span class="sxs-lookup"><span data-stu-id="868c9-127">String</span></span>                      | <span data-ttu-id="868c9-128">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="868c9-128">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="868c9-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="868c9-129">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="868c9-130">Relações</span><span class="sxs-lookup"><span data-stu-id="868c9-130">Relationships</span></span>
<span data-ttu-id="868c9-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="868c9-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="868c9-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="868c9-132">JSON representation</span></span>

<span data-ttu-id="868c9-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="868c9-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


