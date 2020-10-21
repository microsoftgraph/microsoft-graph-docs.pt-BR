---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e77322dee3f8d94fe8eaee226dce029133a578d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635191"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="40815-103">tipo de recurso meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="40815-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="40815-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40815-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40815-105">Contém informações sobre um participante de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="40815-105">Contains information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="40815-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40815-106">Properties</span></span>

| <span data-ttu-id="40815-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40815-107">Property</span></span> | <span data-ttu-id="40815-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="40815-108">Type</span></span>                          | <span data-ttu-id="40815-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="40815-109">Description</span></span>                                                                        |
| :------- | :---------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="40815-110">ladrões</span><span class="sxs-lookup"><span data-stu-id="40815-110">identity</span></span> | [<span data-ttu-id="40815-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="40815-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="40815-112">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="40815-112">Identity information of the participant.</span></span>                                           |
| <span data-ttu-id="40815-113">UPN</span><span class="sxs-lookup"><span data-stu-id="40815-113">upn</span></span>      | <span data-ttu-id="40815-114">String</span><span class="sxs-lookup"><span data-stu-id="40815-114">String</span></span>                        | <span data-ttu-id="40815-115">Nome principal do usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="40815-115">User principal name of the participant.</span></span>                                            |
| <span data-ttu-id="40815-116">role</span><span class="sxs-lookup"><span data-stu-id="40815-116">role</span></span>     | <span data-ttu-id="40815-117">onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="40815-117">onlineMeetingRole</span></span>             | <span data-ttu-id="40815-118">Especifica a função do participante na reunião.</span><span class="sxs-lookup"><span data-stu-id="40815-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="40815-119">Os valores possíveis são: `attendee`, `presenter` e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="40815-119">Possible values are `attendee`, `presenter`, and `unknownFutureValue`.</span></span>|

### <a name="onlinemeetingrole-values"></a><span data-ttu-id="40815-120">valores de onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="40815-120">onlineMeetingRole values</span></span>

| <span data-ttu-id="40815-121">Valor</span><span class="sxs-lookup"><span data-stu-id="40815-121">Value</span></span>              | <span data-ttu-id="40815-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="40815-122">Description</span></span>                     |
| ------------------ | ------------------------------- |
| <span data-ttu-id="40815-123">attendee</span><span class="sxs-lookup"><span data-stu-id="40815-123">attendee</span></span>           | <span data-ttu-id="40815-124">O participante é um participante.</span><span class="sxs-lookup"><span data-stu-id="40815-124">The participant is an attendee.</span></span> |
| <span data-ttu-id="40815-125">instrutor</span><span class="sxs-lookup"><span data-stu-id="40815-125">presenter</span></span>          | <span data-ttu-id="40815-126">O participante é um apresentador.</span><span class="sxs-lookup"><span data-stu-id="40815-126">The participant is a presenter.</span></span> |
| <span data-ttu-id="40815-127">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="40815-127">unknownFutureValue</span></span> | <span data-ttu-id="40815-128">Valor de futuro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="40815-128">Unknown future value.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="40815-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40815-129">JSON representation</span></span>

<span data-ttu-id="40815-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40815-130">The following is a JSON representation of the resource.</span></span>

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


