---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1bc49a3fbf494e378ec695af1f53c0ca4ea313ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521618"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="9f77e-103">tipo de recurso playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="9f77e-103">playPromptOperation resource type</span></span>

<span data-ttu-id="9f77e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f77e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f77e-105">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="9f77e-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="9f77e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f77e-106">Properties</span></span>

| <span data-ttu-id="9f77e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f77e-107">Property</span></span>            | <span data-ttu-id="9f77e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f77e-108">Type</span></span>                        | <span data-ttu-id="9f77e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f77e-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="9f77e-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="9f77e-110">clientContext</span></span>       | <span data-ttu-id="9f77e-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f77e-111">String</span></span>                      | <span data-ttu-id="9f77e-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="9f77e-112">Unique Client Context string.</span></span> <span data-ttu-id="9f77e-113">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="9f77e-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="9f77e-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="9f77e-114">completionReason</span></span>    | <span data-ttu-id="9f77e-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f77e-115">String</span></span>                      | <span data-ttu-id="9f77e-116">Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="9f77e-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="9f77e-117">id</span><span class="sxs-lookup"><span data-stu-id="9f77e-117">id</span></span>                  | <span data-ttu-id="9f77e-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f77e-118">String</span></span>                      | <span data-ttu-id="9f77e-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f77e-119">Read-only.</span></span>                                                                         |
| <span data-ttu-id="9f77e-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9f77e-120">resultInfo</span></span>          | [<span data-ttu-id="9f77e-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9f77e-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="9f77e-122">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="9f77e-122">The result information.</span></span> <span data-ttu-id="9f77e-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f77e-123">Read-only.</span></span>                                |
| <span data-ttu-id="9f77e-124">status</span><span class="sxs-lookup"><span data-stu-id="9f77e-124">status</span></span>              | <span data-ttu-id="9f77e-125">String</span><span class="sxs-lookup"><span data-stu-id="9f77e-125">String</span></span>                      | <span data-ttu-id="9f77e-126">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9f77e-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="9f77e-127">Relações</span><span class="sxs-lookup"><span data-stu-id="9f77e-127">Relationships</span></span>
<span data-ttu-id="9f77e-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f77e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f77e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f77e-129">JSON representation</span></span>

<span data-ttu-id="9f77e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f77e-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
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
