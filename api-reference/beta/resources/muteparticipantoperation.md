---
title: Tipo de recurso MuteParticipantOperation
description: Descreve o formato de resposta de uma operação do participante sem som de chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c5d5e716e4d8266d97139c1283415994f6206aea
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006617"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="51aa3-103">Tipo de recurso MuteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="51aa3-103">MuteParticipantOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51aa3-104">Descreve o formato de resposta de uma operação do participante sem som de chamada.</span><span class="sxs-lookup"><span data-stu-id="51aa3-104">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="51aa3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51aa3-105">Properties</span></span>

| <span data-ttu-id="51aa3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51aa3-106">Property</span></span>                       | <span data-ttu-id="51aa3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="51aa3-107">Type</span></span>                        | <span data-ttu-id="51aa3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="51aa3-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="51aa3-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="51aa3-109">clientContext</span></span>                  | <span data-ttu-id="51aa3-110">String</span><span class="sxs-lookup"><span data-stu-id="51aa3-110">String</span></span>                      | <span data-ttu-id="51aa3-111">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="51aa3-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="51aa3-112">id</span><span class="sxs-lookup"><span data-stu-id="51aa3-112">id</span></span>                             | <span data-ttu-id="51aa3-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51aa3-113">String</span></span>                      | <span data-ttu-id="51aa3-114">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="51aa3-114">The server operation ID.</span></span> <span data-ttu-id="51aa3-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51aa3-115">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="51aa3-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="51aa3-116">resultInfo</span></span>                     | [<span data-ttu-id="51aa3-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="51aa3-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="51aa3-118">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="51aa3-118">The result information.</span></span>  <span data-ttu-id="51aa3-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51aa3-119">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="51aa3-120">status</span><span class="sxs-lookup"><span data-stu-id="51aa3-120">status</span></span>                         | <span data-ttu-id="51aa3-121">String</span><span class="sxs-lookup"><span data-stu-id="51aa3-121">String</span></span>                      | <span data-ttu-id="51aa3-122">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="51aa3-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="51aa3-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51aa3-123">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="51aa3-124">Relações</span><span class="sxs-lookup"><span data-stu-id="51aa3-124">Relationships</span></span>
<span data-ttu-id="51aa3-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51aa3-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51aa3-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51aa3-126">JSON representation</span></span>

<span data-ttu-id="51aa3-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51aa3-127">The following is a JSON representation of the resource.</span></span>

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
