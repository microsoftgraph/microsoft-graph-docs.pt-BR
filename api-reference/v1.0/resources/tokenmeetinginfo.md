---
title: tipo de recurso tokenMeetingInfo
description: O tipo tokenMeetingInfo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 786b3d1429d2f081207fa2d81b5f178d3cb5e08d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533445"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="6779d-103">tipo de recurso tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="6779d-103">tokenMeetingInfo resource type</span></span>

<span data-ttu-id="6779d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6779d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6779d-105">Estas são as informações do token que permitem participar de uma reunião existente.</span><span class="sxs-lookup"><span data-stu-id="6779d-105">This is the token information that allows you to join an existing meeting.</span></span> <span data-ttu-id="6779d-106">Isso é obtido como parte da notificação de chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="6779d-106">This is obtained as part of the incoming call notification.</span></span> 

<span data-ttu-id="6779d-107">No caso de uma chamada ser desconectada, essas informações podem ajudá-lo a reingressar nessa chamada.</span><span class="sxs-lookup"><span data-stu-id="6779d-107">In the event that a call is disconnected, this information can help you rejoin that call.</span></span>

## <a name="properties"></a><span data-ttu-id="6779d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6779d-108">Properties</span></span>

| <span data-ttu-id="6779d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6779d-109">Property</span></span>                     | <span data-ttu-id="6779d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6779d-110">Type</span></span>    | <span data-ttu-id="6779d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6779d-111">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="6779d-112">token</span><span class="sxs-lookup"><span data-stu-id="6779d-112">token</span></span>                        | <span data-ttu-id="6779d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6779d-113">String</span></span>  | <span data-ttu-id="6779d-114">O token usado para ingressar na chamada.</span><span class="sxs-lookup"><span data-stu-id="6779d-114">The token used to join the call.</span></span>                                                 |

## <a name="json-representation"></a><span data-ttu-id="6779d-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6779d-115">JSON representation</span></span>

<span data-ttu-id="6779d-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6779d-116">The following is a JSON representation of the resource.</span></span>

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
