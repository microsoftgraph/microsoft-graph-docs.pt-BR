---
title: tipo de recurso updateRecordingStatusOperation
description: Descreve o formato de resposta de uma ação de status de gravação de atualização.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 302ea2c5ce0cfb54168bf936f8c6e5829e0867c7
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913279"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="bceca-103">tipo de recurso updateRecordingStatusOperation</span><span class="sxs-lookup"><span data-stu-id="bceca-103">updateRecordingStatusOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bceca-104">Descreve o formato de resposta de uma ação de status de gravação de atualização.</span><span class="sxs-lookup"><span data-stu-id="bceca-104">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="bceca-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bceca-105">Properties</span></span>

| <span data-ttu-id="bceca-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bceca-106">Property</span></span>            | <span data-ttu-id="bceca-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bceca-107">Type</span></span>                        | <span data-ttu-id="bceca-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bceca-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="bceca-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="bceca-109">clientContext</span></span>       | <span data-ttu-id="bceca-110">String</span><span class="sxs-lookup"><span data-stu-id="bceca-110">String</span></span>                      | <span data-ttu-id="bceca-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="bceca-111">Unique Client Context string.</span></span> <span data-ttu-id="bceca-112">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="bceca-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="bceca-113">id</span><span class="sxs-lookup"><span data-stu-id="bceca-113">id</span></span>                  | <span data-ttu-id="bceca-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bceca-114">String</span></span>                      | <span data-ttu-id="bceca-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bceca-115">Read-only.</span></span>                                                                         |
| <span data-ttu-id="bceca-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="bceca-116">resultInfo</span></span>          | [<span data-ttu-id="bceca-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="bceca-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="bceca-118">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="bceca-118">The result information.</span></span> <span data-ttu-id="bceca-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bceca-119">Read-only.</span></span>                                                 |
| <span data-ttu-id="bceca-120">status</span><span class="sxs-lookup"><span data-stu-id="bceca-120">status</span></span>              | <span data-ttu-id="bceca-121">String</span><span class="sxs-lookup"><span data-stu-id="bceca-121">String</span></span>                      | <span data-ttu-id="bceca-122">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="bceca-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="bceca-123">Relações</span><span class="sxs-lookup"><span data-stu-id="bceca-123">Relationships</span></span>
<span data-ttu-id="bceca-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bceca-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bceca-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bceca-125">JSON representation</span></span>

<span data-ttu-id="bceca-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bceca-126">The following is a JSON representation of the resource.</span></span>

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
