---
title: tipo de recurso unmuteParticipantOperation
description: Descreve o formato de resposta de uma chamada operação de desativação de participantes.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4a3a4428f1c7be9a840b18625b788b26751eca57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090631"
---
# <a name="unmuteparticipantoperation-resource-type"></a><span data-ttu-id="c03ff-103">tipo de recurso unmuteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="c03ff-103">unmuteParticipantOperation resource type</span></span>

<span data-ttu-id="c03ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c03ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c03ff-105">Descreve o formato de resposta de uma chamada operação de desativação de participantes.</span><span class="sxs-lookup"><span data-stu-id="c03ff-105">Describes the response format of a call participant unmute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="c03ff-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c03ff-106">Properties</span></span>

| <span data-ttu-id="c03ff-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c03ff-107">Property</span></span>                       | <span data-ttu-id="c03ff-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c03ff-108">Type</span></span>                        | <span data-ttu-id="c03ff-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c03ff-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c03ff-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="c03ff-110">clientContext</span></span>                  | <span data-ttu-id="c03ff-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c03ff-111">String</span></span>                      | <span data-ttu-id="c03ff-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="c03ff-112">Unique client context string.</span></span> <span data-ttu-id="c03ff-113">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c03ff-113">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="c03ff-114">id</span><span class="sxs-lookup"><span data-stu-id="c03ff-114">id</span></span>                             | <span data-ttu-id="c03ff-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c03ff-115">String</span></span>                      | <span data-ttu-id="c03ff-116">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="c03ff-116">The server operation ID.</span></span> <span data-ttu-id="c03ff-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c03ff-117">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="c03ff-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c03ff-118">resultInfo</span></span>                     | [<span data-ttu-id="c03ff-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c03ff-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c03ff-120">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="c03ff-120">The result information.</span></span>  <span data-ttu-id="c03ff-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c03ff-121">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="c03ff-122">status</span><span class="sxs-lookup"><span data-stu-id="c03ff-122">status</span></span>                         | <span data-ttu-id="c03ff-123">String</span><span class="sxs-lookup"><span data-stu-id="c03ff-123">String</span></span>                      | <span data-ttu-id="c03ff-124">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c03ff-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c03ff-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c03ff-125">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="c03ff-126">Relações</span><span class="sxs-lookup"><span data-stu-id="c03ff-126">Relationships</span></span>
<span data-ttu-id="c03ff-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c03ff-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c03ff-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c03ff-128">JSON representation</span></span>

<span data-ttu-id="c03ff-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c03ff-129">The following is a JSON representation of the resource.</span></span>

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

