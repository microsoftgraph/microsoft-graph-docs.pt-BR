---
title: tipo de recurso meetingInfo
description: Informações de reunião especificadas para criar ou ingressar em uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ef9c2b86c9eb745ae6282a5d3cbce8a76dc31139
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006638"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="8f956-103">tipo de recurso meetingInfo</span><span class="sxs-lookup"><span data-stu-id="8f956-103">meetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f956-104">Esta é uma classe abstrata que contém informações específicas da reunião.</span><span class="sxs-lookup"><span data-stu-id="8f956-104">This is an abstract class that contains meeting specific information.</span></span>
 
<span data-ttu-id="8f956-105">Para ingressar em uma reunião existente, você deve especificar o [organizerMeetingInfo](organizermeetinginfo.md) em combinação com o [chatInfo](./chatinfo.md)ou apenas o [tokenMeetingInfo](tokenmeetinginfo.md).</span><span class="sxs-lookup"><span data-stu-id="8f956-105">To join an existing meeting, you must either specify the [organizerMeetingInfo](organizermeetinginfo.md) in combination with the [chatInfo](./chatinfo.md), or just the the [tokenMeetingInfo](tokenmeetinginfo.md).</span></span>


## <a name="derived-types"></a><span data-ttu-id="8f956-106">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="8f956-106">Derived types</span></span>

| <span data-ttu-id="8f956-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f956-107">Type</span></span>                                                 | <span data-ttu-id="8f956-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f956-108">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="8f956-109">organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="8f956-109">organizerMeetingInfo</span></span>](./organizermeetinginfo.md)    | <span data-ttu-id="8f956-110">Detalhes sobre o organizador da reunião</span><span class="sxs-lookup"><span data-stu-id="8f956-110">Details about the organizer of the meeting</span></span>                          |
| [<span data-ttu-id="8f956-111">tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="8f956-111">tokenMeetingInfo</span></span>](tokenmeetinginfo.md)              | <span data-ttu-id="8f956-112">Um token criptografado que contém as informações sobre a reunião</span><span class="sxs-lookup"><span data-stu-id="8f956-112">An encrypted token that contains the information about the meeting</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8f956-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f956-113">JSON representation</span></span>

<span data-ttu-id="8f956-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f956-114">The following is a JSON representation of the resource.</span></span>

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
