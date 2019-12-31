---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 731e8597fba4347659a3cddea8fb2934258255c7
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913216"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="53640-103">tipo de recurso playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="53640-103">playPromptOperation resource type</span></span>

<span data-ttu-id="53640-104">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="53640-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="53640-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53640-105">Properties</span></span>

| <span data-ttu-id="53640-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53640-106">Property</span></span>            | <span data-ttu-id="53640-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="53640-107">Type</span></span>                        | <span data-ttu-id="53640-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="53640-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="53640-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="53640-109">clientContext</span></span>       | <span data-ttu-id="53640-110">String</span><span class="sxs-lookup"><span data-stu-id="53640-110">String</span></span>                      | <span data-ttu-id="53640-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="53640-111">Unique Client Context string.</span></span> <span data-ttu-id="53640-112">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="53640-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="53640-113">id</span><span class="sxs-lookup"><span data-stu-id="53640-113">id</span></span>                  | <span data-ttu-id="53640-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53640-114">String</span></span>                      | <span data-ttu-id="53640-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53640-115">Read-only.</span></span>                                                                         |
| <span data-ttu-id="53640-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="53640-116">resultInfo</span></span>          | [<span data-ttu-id="53640-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="53640-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="53640-118">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="53640-118">The result information.</span></span> <span data-ttu-id="53640-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53640-119">Read-only.</span></span>                                |
| <span data-ttu-id="53640-120">status</span><span class="sxs-lookup"><span data-stu-id="53640-120">status</span></span>              | <span data-ttu-id="53640-121">String</span><span class="sxs-lookup"><span data-stu-id="53640-121">String</span></span>                      | <span data-ttu-id="53640-122">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="53640-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="53640-123">Relações</span><span class="sxs-lookup"><span data-stu-id="53640-123">Relationships</span></span>
<span data-ttu-id="53640-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53640-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53640-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53640-125">JSON representation</span></span>

<span data-ttu-id="53640-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53640-126">The following is a JSON representation of the resource.</span></span>

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
