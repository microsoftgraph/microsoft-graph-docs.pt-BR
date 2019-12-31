---
title: tipo de recurso tokenMeetingInfo
description: O tipo tokenMeetingInfo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05cc4c21fe3a8ea0d4b27b6c27b737ec6fe317d2
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912969"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="e8658-103">tipo de recurso tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="e8658-103">tokenMeetingInfo resource type</span></span>

<span data-ttu-id="e8658-104">Estas são as informações do token que permitem participar de uma reunião existente.</span><span class="sxs-lookup"><span data-stu-id="e8658-104">This is the token information that allows you to join an existing meeting.</span></span> <span data-ttu-id="e8658-105">Isso é obtido como parte da notificação de chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="e8658-105">This is obtained as part of the incoming call notification.</span></span> 

<span data-ttu-id="e8658-106">No caso de uma chamada ser desconectada, essas informações podem ajudá-lo a reingressar nessa chamada.</span><span class="sxs-lookup"><span data-stu-id="e8658-106">In the event that a call is disconnected, this information can help you rejoin that call.</span></span>

## <a name="properties"></a><span data-ttu-id="e8658-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8658-107">Properties</span></span>

| <span data-ttu-id="e8658-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8658-108">Property</span></span>                     | <span data-ttu-id="e8658-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8658-109">Type</span></span>    | <span data-ttu-id="e8658-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8658-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="e8658-111">token</span><span class="sxs-lookup"><span data-stu-id="e8658-111">token</span></span>                        | <span data-ttu-id="e8658-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8658-112">String</span></span>  | <span data-ttu-id="e8658-113">O token usado para ingressar na chamada.</span><span class="sxs-lookup"><span data-stu-id="e8658-113">The token used to join the call.</span></span>                                                 |

## <a name="json-representation"></a><span data-ttu-id="e8658-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8658-114">JSON representation</span></span>

<span data-ttu-id="e8658-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8658-115">The following is a JSON representation of the resource.</span></span>

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
