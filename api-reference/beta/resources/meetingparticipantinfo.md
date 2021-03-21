---
title: Tipo de recurso meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 03d2c207d8c64d3e8b63dae223b624f575b193fd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956944"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="bac92-103">Tipo de recurso meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="bac92-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="bac92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bac92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bac92-105">Contém informações sobre um participante em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="bac92-105">Contains information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="bac92-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bac92-106">Properties</span></span>

| <span data-ttu-id="bac92-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bac92-107">Property</span></span> | <span data-ttu-id="bac92-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bac92-108">Type</span></span>                          | <span data-ttu-id="bac92-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bac92-109">Description</span></span>                                                                        |
| :------- | :---------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="bac92-110">identity</span><span class="sxs-lookup"><span data-stu-id="bac92-110">identity</span></span> | [<span data-ttu-id="bac92-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="bac92-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="bac92-112">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="bac92-112">Identity information of the participant.</span></span>                                           |
| <span data-ttu-id="bac92-113">upn</span><span class="sxs-lookup"><span data-stu-id="bac92-113">upn</span></span>      | <span data-ttu-id="bac92-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bac92-114">String</span></span>                        | <span data-ttu-id="bac92-115">Nome principal do usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="bac92-115">User principal name of the participant.</span></span>                                            |
| <span data-ttu-id="bac92-116">role</span><span class="sxs-lookup"><span data-stu-id="bac92-116">role</span></span>     | <span data-ttu-id="bac92-117">onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="bac92-117">onlineMeetingRole</span></span>             | <span data-ttu-id="bac92-118">Especifica a função do participante na reunião.</span><span class="sxs-lookup"><span data-stu-id="bac92-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="bac92-119">Os valores possíveis `attendee` `presenter` são , e `producer` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="bac92-119">Possible values are `attendee`, `presenter`, `producer`, and `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bac92-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bac92-120">JSON representation</span></span>

<span data-ttu-id="bac92-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bac92-121">The following is a JSON representation of the resource.</span></span>

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


