---
title: tipo de recurso organizerMeetingInfo
description: 'Contém detalhes sobre o organizador da reunião. '
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab1d907365e40b70a8d85a845c9e8ec0366183af
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870986"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="0eebe-103">tipo de recurso organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="0eebe-103">organizerMeetingInfo resource type</span></span>

<span data-ttu-id="0eebe-104">Contém detalhes sobre o organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="0eebe-104">Contains details about the meeting organizer.</span></span> 

<span data-ttu-id="0eebe-105">Para ingressar em uma reunião existente, você deve fornecer uma combinação dos tipos de recurso organizerMeetingInfo e [chatInfo](./chatinfo.md) ou o tipo de recurso [tokenMeetingInfo](./tokenmeetinginfo.md) sozinho.</span><span class="sxs-lookup"><span data-stu-id="0eebe-105">To join an existing meeting, you must either provide a combination of the organizerMeetingInfo and the [chatInfo](./chatinfo.md) resource types, or the [tokenMeetingInfo](./tokenmeetinginfo.md) resource type by itself.</span></span>

## <a name="properties"></a><span data-ttu-id="0eebe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0eebe-106">Properties</span></span>

| <span data-ttu-id="0eebe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0eebe-107">Property</span></span>                     | <span data-ttu-id="0eebe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0eebe-108">Type</span></span>                          | <span data-ttu-id="0eebe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0eebe-109">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="0eebe-110">organizer</span><span class="sxs-lookup"><span data-stu-id="0eebe-110">organizer</span></span>                    | [<span data-ttu-id="0eebe-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="0eebe-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="0eebe-112">A identidade do Azure Active Directory do organizador.</span><span class="sxs-lookup"><span data-stu-id="0eebe-112">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0eebe-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0eebe-113">JSON representation</span></span>

<span data-ttu-id="0eebe-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0eebe-114">The following is a JSON representation of the resource.</span></span>

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
