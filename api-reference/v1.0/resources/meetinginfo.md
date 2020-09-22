---
title: tipo de recurso meetingInfo
description: Informações de reunião especificadas para criar ou ingressar em uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cb79cae4f413e3d027b8dbbcccc621ba9b3b8233
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020542"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="9d225-103">tipo de recurso meetingInfo</span><span class="sxs-lookup"><span data-stu-id="9d225-103">meetingInfo resource type</span></span>

<span data-ttu-id="9d225-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d225-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d225-105">Esta é uma classe abstrata que contém informações específicas da reunião.</span><span class="sxs-lookup"><span data-stu-id="9d225-105">This is an abstract class that contains meeting specific information.</span></span>
 
<span data-ttu-id="9d225-106">Para ingressar em uma reunião existente, você deve especificar o [organizerMeetingInfo](organizermeetinginfo.md) em combinação com o [chatInfo](./chatinfo.md)ou apenas o [tokenMeetingInfo](tokenmeetinginfo.md).</span><span class="sxs-lookup"><span data-stu-id="9d225-106">To join an existing meeting, you must either specify the [organizerMeetingInfo](organizermeetinginfo.md) in combination with the [chatInfo](./chatinfo.md), or just the [tokenMeetingInfo](tokenmeetinginfo.md).</span></span>


## <a name="derived-types"></a><span data-ttu-id="9d225-107">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="9d225-107">Derived types</span></span>

| <span data-ttu-id="9d225-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d225-108">Type</span></span>                                                 | <span data-ttu-id="9d225-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d225-109">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="9d225-110">organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="9d225-110">organizerMeetingInfo</span></span>](./organizermeetinginfo.md)    | <span data-ttu-id="9d225-111">Detalhes sobre o organizador da reunião</span><span class="sxs-lookup"><span data-stu-id="9d225-111">Details about the organizer of the meeting</span></span>                          |
| [<span data-ttu-id="9d225-112">tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="9d225-112">tokenMeetingInfo</span></span>](tokenmeetinginfo.md)              | <span data-ttu-id="9d225-113">Um token criptografado que contém as informações sobre a reunião</span><span class="sxs-lookup"><span data-stu-id="9d225-113">An encrypted token that contains the information about the meeting</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9d225-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d225-114">JSON representation</span></span>

<span data-ttu-id="9d225-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d225-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

