---
title: tipo de recurso updateRecordingStatusOperation
description: Descreve o formato de resposta de uma ação de status de gravação de atualização.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 92cfc481d10cccd3752db29a0c1da7d46000ed3b
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636916"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="6a22f-103">tipo de recurso updateRecordingStatusOperation</span><span class="sxs-lookup"><span data-stu-id="6a22f-103">updateRecordingStatusOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a22f-104">Descreve o formato de resposta de uma ação de status de gravação de atualização.</span><span class="sxs-lookup"><span data-stu-id="6a22f-104">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="6a22f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a22f-105">Properties</span></span>

| <span data-ttu-id="6a22f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a22f-106">Property</span></span>            | <span data-ttu-id="6a22f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a22f-107">Type</span></span>                        | <span data-ttu-id="6a22f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a22f-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="6a22f-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="6a22f-109">clientContext</span></span>       | <span data-ttu-id="6a22f-110">String</span><span class="sxs-lookup"><span data-stu-id="6a22f-110">String</span></span>                      | <span data-ttu-id="6a22f-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="6a22f-111">Unique Client Context string.</span></span> <span data-ttu-id="6a22f-112">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6a22f-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="6a22f-113">id</span><span class="sxs-lookup"><span data-stu-id="6a22f-113">id</span></span>                  | <span data-ttu-id="6a22f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a22f-114">String</span></span>                      | <span data-ttu-id="6a22f-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a22f-115">Read-only.</span></span>                                                                         |
| <span data-ttu-id="6a22f-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6a22f-116">resultInfo</span></span>          | [<span data-ttu-id="6a22f-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6a22f-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="6a22f-118">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="6a22f-118">The result information.</span></span> <span data-ttu-id="6a22f-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a22f-119">Read-only.</span></span>                                                 |
| <span data-ttu-id="6a22f-120">status</span><span class="sxs-lookup"><span data-stu-id="6a22f-120">status</span></span>              | <span data-ttu-id="6a22f-121">String</span><span class="sxs-lookup"><span data-stu-id="6a22f-121">String</span></span>                      | <span data-ttu-id="6a22f-122">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6a22f-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="6a22f-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6a22f-123">Relationships</span></span>
<span data-ttu-id="6a22f-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a22f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a22f-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a22f-125">JSON representation</span></span>

<span data-ttu-id="6a22f-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a22f-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
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
  "description": "updateRecordingStatusOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
