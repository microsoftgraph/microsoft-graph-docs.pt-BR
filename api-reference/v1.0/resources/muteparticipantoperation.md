---
title: Tipo de recurso MuteParticipantOperation
description: Descreve o formato de resposta de uma operação do participante sem som de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: eb85ea8e1759dc948f764b391e25a51b97090566
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447371"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="f4a99-103">Tipo de recurso MuteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="f4a99-103">MuteParticipantOperation resource type</span></span>

<span data-ttu-id="f4a99-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f4a99-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4a99-105">Descreve o formato de resposta de uma operação do participante sem som de chamada.</span><span class="sxs-lookup"><span data-stu-id="f4a99-105">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="f4a99-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4a99-106">Properties</span></span>

| <span data-ttu-id="f4a99-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4a99-107">Property</span></span>                       | <span data-ttu-id="f4a99-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4a99-108">Type</span></span>                        | <span data-ttu-id="f4a99-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4a99-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f4a99-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="f4a99-110">clientContext</span></span>                  | <span data-ttu-id="f4a99-111">String</span><span class="sxs-lookup"><span data-stu-id="f4a99-111">String</span></span>                      | <span data-ttu-id="f4a99-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="f4a99-112">Unique client context string.</span></span> <span data-ttu-id="f4a99-113">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="f4a99-113">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="f4a99-114">id</span><span class="sxs-lookup"><span data-stu-id="f4a99-114">id</span></span>                             | <span data-ttu-id="f4a99-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4a99-115">String</span></span>                      | <span data-ttu-id="f4a99-116">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="f4a99-116">The server operation ID.</span></span> <span data-ttu-id="f4a99-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a99-117">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="f4a99-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f4a99-118">resultInfo</span></span>                     | [<span data-ttu-id="f4a99-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f4a99-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="f4a99-120">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="f4a99-120">The result information.</span></span>  <span data-ttu-id="f4a99-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a99-121">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="f4a99-122">status</span><span class="sxs-lookup"><span data-stu-id="f4a99-122">status</span></span>                         | <span data-ttu-id="f4a99-123">String</span><span class="sxs-lookup"><span data-stu-id="f4a99-123">String</span></span>                      | <span data-ttu-id="f4a99-124">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f4a99-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="f4a99-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a99-125">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="f4a99-126">Relações</span><span class="sxs-lookup"><span data-stu-id="f4a99-126">Relationships</span></span>
<span data-ttu-id="f4a99-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4a99-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4a99-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4a99-128">JSON representation</span></span>

<span data-ttu-id="f4a99-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4a99-129">The following is a JSON representation of the resource.</span></span>

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
