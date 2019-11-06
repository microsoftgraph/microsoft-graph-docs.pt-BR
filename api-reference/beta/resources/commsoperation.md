---
title: tipo de recurso commsOperation
description: O status de determinadas operações de longa duração.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 07be6f3b5cf9e3d5e7a1a1300a94da9b5204a68a
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006695"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="c3236-103">tipo de recurso commsOperation</span><span class="sxs-lookup"><span data-stu-id="c3236-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3236-104">Representa o status de determinadas operações de longa duração.</span><span class="sxs-lookup"><span data-stu-id="c3236-104">Represents the status of certain long-running operations.</span></span>

<span data-ttu-id="c3236-105">Esse recurso pode ser retornado como a resposta a uma ação ou como o conteúdo de um [commsNotification](commsNotification.md).</span><span class="sxs-lookup"><span data-stu-id="c3236-105">This resource can be returned as the response to an action, or as the content of a [commsNotification](commsNotification.md).</span></span>  

<span data-ttu-id="c3236-106">Quando ele é retornado como uma resposta a uma ação, o status indica se haverá notificações subsequentes.</span><span class="sxs-lookup"><span data-stu-id="c3236-106">When it is returned as a response to an action, the status indicates whether there will be subsequent notifications.</span></span> <span data-ttu-id="c3236-107">Se, por exemplo, uma operação com status `completed` ou `failed` for retornada, não haverá nenhuma operação subsequente por meio do canal de notificação.</span><span class="sxs-lookup"><span data-stu-id="c3236-107">If, for example, an operation with status of `completed` or `failed` is returned,  there will not be any subsequent operation via the notification channel.</span></span> 

<span data-ttu-id="c3236-108">Se uma `null` operação ou uma operação com o status `notStarted` ou `running` for retornada, as atualizações subsequentes serão fornecidas pelo canal de notificação.</span><span class="sxs-lookup"><span data-stu-id="c3236-108">If a `null` operation, or an operation with a status of `notStarted` or `running` is returned, subsequent updates will come via the notification channel.</span></span>

## <a name="properties"></a><span data-ttu-id="c3236-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3236-109">Properties</span></span>

| <span data-ttu-id="c3236-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3236-110">Property</span></span>           | <span data-ttu-id="c3236-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3236-111">Type</span></span>                        | <span data-ttu-id="c3236-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3236-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="c3236-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="c3236-113">clientContext</span></span>      | <span data-ttu-id="c3236-114">String</span><span class="sxs-lookup"><span data-stu-id="c3236-114">String</span></span>                      | <span data-ttu-id="c3236-115">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="c3236-115">Unique Client Context string.</span></span> <span data-ttu-id="c3236-116">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c3236-116">Max limit is 256 chars.</span></span>                           |
| <span data-ttu-id="c3236-117">id</span><span class="sxs-lookup"><span data-stu-id="c3236-117">id</span></span>                 | <span data-ttu-id="c3236-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3236-118">String</span></span>                      | <span data-ttu-id="c3236-119">A ID da operação.</span><span class="sxs-lookup"><span data-stu-id="c3236-119">The operation ID.</span></span> <span data-ttu-id="c3236-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3236-120">Read-only.</span></span>                                                    |
| <span data-ttu-id="c3236-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c3236-121">resultInfo</span></span>         | [<span data-ttu-id="c3236-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c3236-122">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c3236-123">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="c3236-123">The result information.</span></span> <span data-ttu-id="c3236-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3236-124">Read-only.</span></span>                                              |
| <span data-ttu-id="c3236-125">status</span><span class="sxs-lookup"><span data-stu-id="c3236-125">status</span></span>             | <span data-ttu-id="c3236-126">String</span><span class="sxs-lookup"><span data-stu-id="c3236-126">String</span></span>                      | <span data-ttu-id="c3236-127">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c3236-127">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c3236-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3236-128">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c3236-129">Relações</span><span class="sxs-lookup"><span data-stu-id="c3236-129">Relationships</span></span>
<span data-ttu-id="c3236-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3236-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3236-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3236-131">JSON representation</span></span>

<span data-ttu-id="c3236-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3236-132">The following is a JSON representation of the resource.</span></span>

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
