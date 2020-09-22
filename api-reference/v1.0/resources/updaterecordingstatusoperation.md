---
title: tipo de recurso updateRecordingStatusOperation
description: Descreve o formato de resposta de uma ação de status de gravação de atualização.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 78c5e91fa966a91bc65291fa813807cdf44ee8ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090617"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="9f88c-103">tipo de recurso updateRecordingStatusOperation</span><span class="sxs-lookup"><span data-stu-id="9f88c-103">updateRecordingStatusOperation resource type</span></span>

<span data-ttu-id="9f88c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f88c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f88c-105">Descreve o formato de resposta de uma ação de status de gravação de atualização.</span><span class="sxs-lookup"><span data-stu-id="9f88c-105">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="9f88c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f88c-106">Properties</span></span>

| <span data-ttu-id="9f88c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f88c-107">Property</span></span>            | <span data-ttu-id="9f88c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f88c-108">Type</span></span>                        | <span data-ttu-id="9f88c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f88c-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="9f88c-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="9f88c-110">clientContext</span></span>       | <span data-ttu-id="9f88c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f88c-111">String</span></span>                      | <span data-ttu-id="9f88c-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="9f88c-112">Unique client context string.</span></span> <span data-ttu-id="9f88c-113">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="9f88c-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="9f88c-114">id</span><span class="sxs-lookup"><span data-stu-id="9f88c-114">id</span></span>                  | <span data-ttu-id="9f88c-115">String</span><span class="sxs-lookup"><span data-stu-id="9f88c-115">String</span></span>                      | <span data-ttu-id="9f88c-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f88c-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="9f88c-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9f88c-117">resultInfo</span></span>          | [<span data-ttu-id="9f88c-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9f88c-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="9f88c-119">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="9f88c-119">The result information.</span></span> <span data-ttu-id="9f88c-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f88c-120">Read-only.</span></span>                                                 |
| <span data-ttu-id="9f88c-121">status</span><span class="sxs-lookup"><span data-stu-id="9f88c-121">status</span></span>              | <span data-ttu-id="9f88c-122">String</span><span class="sxs-lookup"><span data-stu-id="9f88c-122">String</span></span>                      | <span data-ttu-id="9f88c-123">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9f88c-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="9f88c-124">Relações</span><span class="sxs-lookup"><span data-stu-id="9f88c-124">Relationships</span></span>
<span data-ttu-id="9f88c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f88c-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f88c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f88c-126">JSON representation</span></span>

<span data-ttu-id="9f88c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f88c-127">The following is a JSON representation of the resource.</span></span>

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

