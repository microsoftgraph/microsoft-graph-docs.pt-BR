---
title: tipo de recurso meetingInfo
description: Informações de reunião especificadas para criar ou ingressar em uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1c6bda0463b2762122695ed84ecc02c1b5dd3d1b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522733"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="abb0c-103">tipo de recurso meetingInfo</span><span class="sxs-lookup"><span data-stu-id="abb0c-103">meetingInfo resource type</span></span>

<span data-ttu-id="abb0c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="abb0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abb0c-105">Esta é uma classe abstrata que contém informações específicas da reunião.</span><span class="sxs-lookup"><span data-stu-id="abb0c-105">This is an abstract class that contains meeting specific information.</span></span>
 
<span data-ttu-id="abb0c-106">Para ingressar em uma reunião existente, você deve especificar o [organizerMeetingInfo](organizermeetinginfo.md) em combinação com o [chatInfo](./chatinfo.md)ou apenas o [tokenMeetingInfo](tokenmeetinginfo.md).</span><span class="sxs-lookup"><span data-stu-id="abb0c-106">To join an existing meeting, you must either specify the [organizerMeetingInfo](organizermeetinginfo.md) in combination with the [chatInfo](./chatinfo.md), or just the the [tokenMeetingInfo](tokenmeetinginfo.md).</span></span>


## <a name="derived-types"></a><span data-ttu-id="abb0c-107">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="abb0c-107">Derived types</span></span>

| <span data-ttu-id="abb0c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="abb0c-108">Type</span></span>                                                 | <span data-ttu-id="abb0c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="abb0c-109">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="abb0c-110">organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="abb0c-110">organizerMeetingInfo</span></span>](./organizermeetinginfo.md)    | <span data-ttu-id="abb0c-111">Detalhes sobre o organizador da reunião</span><span class="sxs-lookup"><span data-stu-id="abb0c-111">Details about the organizer of the meeting</span></span>                          |
| [<span data-ttu-id="abb0c-112">tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="abb0c-112">tokenMeetingInfo</span></span>](tokenmeetinginfo.md)              | <span data-ttu-id="abb0c-113">Um token criptografado que contém as informações sobre a reunião</span><span class="sxs-lookup"><span data-stu-id="abb0c-113">An encrypted token that contains the information about the meeting</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="abb0c-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abb0c-114">JSON representation</span></span>

<span data-ttu-id="abb0c-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abb0c-115">The following is a JSON representation of the resource.</span></span>

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
