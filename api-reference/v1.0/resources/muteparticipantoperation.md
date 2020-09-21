---
title: Tipo de recurso MuteParticipantOperation
description: Descreve o formato de resposta de uma operação do participante sem som de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 51806154a36433ee054250bc1c306b64953a8766
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967370"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="ea477-103">Tipo de recurso MuteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="ea477-103">MuteParticipantOperation resource type</span></span>

<span data-ttu-id="ea477-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea477-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea477-105">Descreve o formato de resposta de uma operação do participante sem som de chamada.</span><span class="sxs-lookup"><span data-stu-id="ea477-105">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="ea477-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea477-106">Properties</span></span>

| <span data-ttu-id="ea477-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea477-107">Property</span></span>                       | <span data-ttu-id="ea477-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea477-108">Type</span></span>                        | <span data-ttu-id="ea477-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea477-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ea477-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="ea477-110">clientContext</span></span>                  | <span data-ttu-id="ea477-111">String</span><span class="sxs-lookup"><span data-stu-id="ea477-111">String</span></span>                      | <span data-ttu-id="ea477-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="ea477-112">Unique client context string.</span></span> <span data-ttu-id="ea477-113">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="ea477-113">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="ea477-114">id</span><span class="sxs-lookup"><span data-stu-id="ea477-114">id</span></span>                             | <span data-ttu-id="ea477-115">String</span><span class="sxs-lookup"><span data-stu-id="ea477-115">String</span></span>                      | <span data-ttu-id="ea477-116">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="ea477-116">The server operation ID.</span></span> <span data-ttu-id="ea477-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea477-117">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="ea477-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ea477-118">resultInfo</span></span>                     | [<span data-ttu-id="ea477-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ea477-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="ea477-120">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="ea477-120">The result information.</span></span>  <span data-ttu-id="ea477-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea477-121">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="ea477-122">status</span><span class="sxs-lookup"><span data-stu-id="ea477-122">status</span></span>                         | <span data-ttu-id="ea477-123">String</span><span class="sxs-lookup"><span data-stu-id="ea477-123">String</span></span>                      | <span data-ttu-id="ea477-124">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ea477-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="ea477-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea477-125">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="ea477-126">Relações</span><span class="sxs-lookup"><span data-stu-id="ea477-126">Relationships</span></span>
<span data-ttu-id="ea477-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea477-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea477-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea477-128">JSON representation</span></span>

<span data-ttu-id="ea477-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea477-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.muteParticipantOperation"
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
  "description": "muteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

