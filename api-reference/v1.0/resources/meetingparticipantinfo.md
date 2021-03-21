---
title: Tipo de recurso meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 40209354f1621839bd51a20fcbafa4cd58b4fd8d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962452"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="7cd18-103">Tipo de recurso meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="7cd18-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="7cd18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cd18-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7cd18-105">Informações sobre um participante em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="7cd18-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="7cd18-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7cd18-106">Properties</span></span>

| <span data-ttu-id="7cd18-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7cd18-107">Property</span></span> | <span data-ttu-id="7cd18-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cd18-108">Type</span></span>                          | <span data-ttu-id="7cd18-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cd18-109">Description</span></span>                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| <span data-ttu-id="7cd18-110">identity</span><span class="sxs-lookup"><span data-stu-id="7cd18-110">identity</span></span> | [<span data-ttu-id="7cd18-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="7cd18-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="7cd18-112">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="7cd18-112">Identity information of the participant.</span></span>                                            |
| <span data-ttu-id="7cd18-113">upn</span><span class="sxs-lookup"><span data-stu-id="7cd18-113">upn</span></span>      | <span data-ttu-id="7cd18-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cd18-114">String</span></span>                        | <span data-ttu-id="7cd18-115">Nome principal do usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="7cd18-115">User principal name of the participant.</span></span>                                             |
| <span data-ttu-id="7cd18-116">role</span><span class="sxs-lookup"><span data-stu-id="7cd18-116">role</span></span>     | <span data-ttu-id="7cd18-117">onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="7cd18-117">onlineMeetingRole</span></span>             | <span data-ttu-id="7cd18-118">Especifica a função do participante na reunião.</span><span class="sxs-lookup"><span data-stu-id="7cd18-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="7cd18-119">Os valores possíveis são: `attendee`, `presenter` e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7cd18-119">Possible values are `attendee`, `presenter`, and `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cd18-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7cd18-120">JSON representation</span></span>

<span data-ttu-id="7cd18-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7cd18-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String",
  "role": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

