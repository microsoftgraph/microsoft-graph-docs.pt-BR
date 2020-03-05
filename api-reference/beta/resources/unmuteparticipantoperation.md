---
title: tipo de recurso unmuteParticipantOperation
description: Descreve o formato de resposta de uma chamada operação de desativação de participantes.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d9ebb8d749f8cbe6ce01711ca6a0c36b134e8369
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519593"
---
# <a name="unmuteparticipantoperation-resource-type"></a><span data-ttu-id="155c9-103">tipo de recurso unmuteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="155c9-103">unmuteParticipantOperation resource type</span></span>

<span data-ttu-id="155c9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="155c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="155c9-105">Descreve o formato de resposta de uma chamada operação de desativação de participantes.</span><span class="sxs-lookup"><span data-stu-id="155c9-105">Describes the response format of a call participant unmute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="155c9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="155c9-106">Properties</span></span>

| <span data-ttu-id="155c9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="155c9-107">Property</span></span>                       | <span data-ttu-id="155c9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="155c9-108">Type</span></span>                        | <span data-ttu-id="155c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="155c9-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="155c9-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="155c9-110">clientContext</span></span>                  | <span data-ttu-id="155c9-111">String</span><span class="sxs-lookup"><span data-stu-id="155c9-111">String</span></span>                      | <span data-ttu-id="155c9-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="155c9-112">Unique client context string.</span></span> <span data-ttu-id="155c9-113">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="155c9-113">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="155c9-114">id</span><span class="sxs-lookup"><span data-stu-id="155c9-114">id</span></span>                             | <span data-ttu-id="155c9-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="155c9-115">String</span></span>                      | <span data-ttu-id="155c9-116">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="155c9-116">The server operation ID.</span></span> <span data-ttu-id="155c9-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="155c9-117">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="155c9-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="155c9-118">resultInfo</span></span>                     | [<span data-ttu-id="155c9-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="155c9-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="155c9-120">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="155c9-120">The result information.</span></span>  <span data-ttu-id="155c9-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="155c9-121">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="155c9-122">status</span><span class="sxs-lookup"><span data-stu-id="155c9-122">status</span></span>                         | <span data-ttu-id="155c9-123">String</span><span class="sxs-lookup"><span data-stu-id="155c9-123">String</span></span>                      | <span data-ttu-id="155c9-124">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="155c9-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="155c9-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="155c9-125">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="155c9-126">Relações</span><span class="sxs-lookup"><span data-stu-id="155c9-126">Relationships</span></span>
<span data-ttu-id="155c9-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="155c9-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="155c9-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="155c9-128">JSON representation</span></span>

<span data-ttu-id="155c9-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="155c9-129">The following is a JSON representation of the resource.</span></span>

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
