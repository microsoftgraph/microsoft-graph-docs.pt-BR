---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ae7b1f33216d2d9ae9d867fca57fe2dd27e2e4df
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865649"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="35fe3-103">tipo de recurso playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="35fe3-103">playPromptOperation resource type</span></span>

<span data-ttu-id="35fe3-104">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="35fe3-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="35fe3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35fe3-105">Properties</span></span>

| <span data-ttu-id="35fe3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35fe3-106">Property</span></span>            | <span data-ttu-id="35fe3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="35fe3-107">Type</span></span>                        | <span data-ttu-id="35fe3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="35fe3-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="35fe3-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="35fe3-109">clientContext</span></span>       | <span data-ttu-id="35fe3-110">String</span><span class="sxs-lookup"><span data-stu-id="35fe3-110">String</span></span>                      | <span data-ttu-id="35fe3-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="35fe3-111">Unique Client Context string.</span></span> <span data-ttu-id="35fe3-112">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="35fe3-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="35fe3-113">id</span><span class="sxs-lookup"><span data-stu-id="35fe3-113">id</span></span>                  | <span data-ttu-id="35fe3-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35fe3-114">String</span></span>                      | <span data-ttu-id="35fe3-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35fe3-115">Read-only.</span></span>                                                                         |
| <span data-ttu-id="35fe3-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="35fe3-116">resultInfo</span></span>          | [<span data-ttu-id="35fe3-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="35fe3-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="35fe3-118">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="35fe3-118">The result information.</span></span> <span data-ttu-id="35fe3-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35fe3-119">Read-only.</span></span>                                |
| <span data-ttu-id="35fe3-120">status</span><span class="sxs-lookup"><span data-stu-id="35fe3-120">status</span></span>              | <span data-ttu-id="35fe3-121">String</span><span class="sxs-lookup"><span data-stu-id="35fe3-121">String</span></span>                      | <span data-ttu-id="35fe3-122">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="35fe3-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="35fe3-123">Relações</span><span class="sxs-lookup"><span data-stu-id="35fe3-123">Relationships</span></span>
<span data-ttu-id="35fe3-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35fe3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35fe3-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35fe3-125">JSON representation</span></span>

<span data-ttu-id="35fe3-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35fe3-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
