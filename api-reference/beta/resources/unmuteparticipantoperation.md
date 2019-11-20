---
title: tipo de recurso unmuteParticipantOperation
description: Descreve o formato de resposta de uma chamada operação de desativação de participantes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d3c843ffcf46d8816f4ad3853d42cb5d0fa34422
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748045"
---
# <a name="unmuteparticipantoperation-resource-type"></a><span data-ttu-id="766fd-103">tipo de recurso unmuteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="766fd-103">unmuteParticipantOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="766fd-104">Descreve o formato de resposta de uma chamada operação de desativação de participantes.</span><span class="sxs-lookup"><span data-stu-id="766fd-104">Describes the response format of a call participant unmute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="766fd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="766fd-105">Properties</span></span>

| <span data-ttu-id="766fd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="766fd-106">Property</span></span>                       | <span data-ttu-id="766fd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="766fd-107">Type</span></span>                        | <span data-ttu-id="766fd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="766fd-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="766fd-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="766fd-109">clientContext</span></span>                  | <span data-ttu-id="766fd-110">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="766fd-110">String</span></span>                      | <span data-ttu-id="766fd-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="766fd-111">Unique client context string.</span></span> <span data-ttu-id="766fd-112">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="766fd-112">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="766fd-113">id</span><span class="sxs-lookup"><span data-stu-id="766fd-113">id</span></span>                             | <span data-ttu-id="766fd-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="766fd-114">String</span></span>                      | <span data-ttu-id="766fd-115">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="766fd-115">The server operation ID.</span></span> <span data-ttu-id="766fd-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="766fd-116">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="766fd-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="766fd-117">resultInfo</span></span>                     | [<span data-ttu-id="766fd-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="766fd-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="766fd-119">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="766fd-119">The result information.</span></span>  <span data-ttu-id="766fd-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="766fd-120">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="766fd-121">status</span><span class="sxs-lookup"><span data-stu-id="766fd-121">status</span></span>                         | <span data-ttu-id="766fd-122">String</span><span class="sxs-lookup"><span data-stu-id="766fd-122">String</span></span>                      | <span data-ttu-id="766fd-123">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="766fd-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="766fd-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="766fd-124">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="766fd-125">Relações</span><span class="sxs-lookup"><span data-stu-id="766fd-125">Relationships</span></span>
<span data-ttu-id="766fd-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="766fd-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="766fd-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="766fd-127">JSON representation</span></span>

<span data-ttu-id="766fd-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="766fd-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
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
<!-- {
  "type": "#page.annotation",
  "description": "unmuteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
