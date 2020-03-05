---
title: tipo de recurso updateRecordingStatusOperation
description: Descreve o formato de resposta de uma ação de status de gravação de atualização.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b27aca68e159775bc9e4559d1ff6d5c005c9929a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519586"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="f2505-103">tipo de recurso updateRecordingStatusOperation</span><span class="sxs-lookup"><span data-stu-id="f2505-103">updateRecordingStatusOperation resource type</span></span>

<span data-ttu-id="f2505-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f2505-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2505-105">Descreve o formato de resposta de uma ação de status de gravação de atualização.</span><span class="sxs-lookup"><span data-stu-id="f2505-105">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="f2505-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2505-106">Properties</span></span>

| <span data-ttu-id="f2505-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2505-107">Property</span></span>            | <span data-ttu-id="f2505-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2505-108">Type</span></span>                        | <span data-ttu-id="f2505-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2505-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="f2505-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="f2505-110">clientContext</span></span>       | <span data-ttu-id="f2505-111">String</span><span class="sxs-lookup"><span data-stu-id="f2505-111">String</span></span>                      | <span data-ttu-id="f2505-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="f2505-112">Unique Client Context string.</span></span> <span data-ttu-id="f2505-113">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="f2505-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="f2505-114">id</span><span class="sxs-lookup"><span data-stu-id="f2505-114">id</span></span>                  | <span data-ttu-id="f2505-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2505-115">String</span></span>                      | <span data-ttu-id="f2505-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2505-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="f2505-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f2505-117">resultInfo</span></span>          | [<span data-ttu-id="f2505-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f2505-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="f2505-119">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="f2505-119">The result information.</span></span> <span data-ttu-id="f2505-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2505-120">Read-only.</span></span>                                                 |
| <span data-ttu-id="f2505-121">status</span><span class="sxs-lookup"><span data-stu-id="f2505-121">status</span></span>              | <span data-ttu-id="f2505-122">String</span><span class="sxs-lookup"><span data-stu-id="f2505-122">String</span></span>                      | <span data-ttu-id="f2505-123">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f2505-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="f2505-124">Relações</span><span class="sxs-lookup"><span data-stu-id="f2505-124">Relationships</span></span>
<span data-ttu-id="f2505-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2505-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2505-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2505-126">JSON representation</span></span>

<span data-ttu-id="f2505-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2505-127">The following is a JSON representation of the resource.</span></span>

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
