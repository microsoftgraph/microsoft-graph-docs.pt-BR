---
title: tipo de recurso organizerMeetingInfo
description: 'Contém detalhes sobre o organizador da reunião. '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d3b1f37e6ac5f33d6d59988054d5abfedf5e68e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066282"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="9e562-103">tipo de recurso organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="9e562-103">organizerMeetingInfo resource type</span></span>

<span data-ttu-id="9e562-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e562-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e562-105">Contém detalhes sobre o organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="9e562-105">Contains details about the meeting organizer.</span></span> 

<span data-ttu-id="9e562-106">Para ingressar em uma reunião existente, você deve fornecer uma combinação dos tipos de recurso organizerMeetingInfo e [chatInfo](./chatinfo.md) ou o tipo de recurso [tokenMeetingInfo](./tokenmeetinginfo.md) sozinho.</span><span class="sxs-lookup"><span data-stu-id="9e562-106">To join an existing meeting, you must either provide a combination of the organizerMeetingInfo and the [chatInfo](./chatinfo.md) resource types, or the [tokenMeetingInfo](./tokenmeetinginfo.md) resource type by itself.</span></span>

## <a name="properties"></a><span data-ttu-id="9e562-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e562-107">Properties</span></span>

| <span data-ttu-id="9e562-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e562-108">Property</span></span>                     | <span data-ttu-id="9e562-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e562-109">Type</span></span>                          | <span data-ttu-id="9e562-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e562-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="9e562-111">organizer</span><span class="sxs-lookup"><span data-stu-id="9e562-111">organizer</span></span>                    | [<span data-ttu-id="9e562-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="9e562-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="9e562-113">A identidade do Azure Active Directory do organizador.</span><span class="sxs-lookup"><span data-stu-id="9e562-113">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9e562-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e562-114">JSON representation</span></span>

<span data-ttu-id="9e562-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e562-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

