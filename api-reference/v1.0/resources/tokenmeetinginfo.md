---
title: tipo de recurso tokenMeetingInfo
description: O tipo tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e34a10b9cd0fb09ff29c2d3373ad51a92109dcea
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865635"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="7dd5a-103">tipo de recurso tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="7dd5a-103">tokenMeetingInfo resource type</span></span>

<span data-ttu-id="7dd5a-104">Estas são as informações do token que permitem participar de uma reunião existente.</span><span class="sxs-lookup"><span data-stu-id="7dd5a-104">This is the token information that allows you to join an existing meeting.</span></span> <span data-ttu-id="7dd5a-105">Isso é obtido como parte da notificação de chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="7dd5a-105">This is obtained as part of the incoming call notification.</span></span> 

<span data-ttu-id="7dd5a-106">No caso de uma chamada ser desconectada, essas informações podem ajudá-lo a reingressar nessa chamada.</span><span class="sxs-lookup"><span data-stu-id="7dd5a-106">In the event that a call is disconnected, this information can help you rejoin that call.</span></span>

## <a name="properties"></a><span data-ttu-id="7dd5a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7dd5a-107">Properties</span></span>

| <span data-ttu-id="7dd5a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dd5a-108">Property</span></span>                     | <span data-ttu-id="7dd5a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dd5a-109">Type</span></span>    | <span data-ttu-id="7dd5a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dd5a-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="7dd5a-111">token</span><span class="sxs-lookup"><span data-stu-id="7dd5a-111">token</span></span>                        | <span data-ttu-id="7dd5a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7dd5a-112">String</span></span>  | <span data-ttu-id="7dd5a-113">O token usado para ingressar na chamada.</span><span class="sxs-lookup"><span data-stu-id="7dd5a-113">The token used to join the call.</span></span>                                                 |

## <a name="json-representation"></a><span data-ttu-id="7dd5a-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7dd5a-114">JSON representation</span></span>

<span data-ttu-id="7dd5a-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7dd5a-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
    "token": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
