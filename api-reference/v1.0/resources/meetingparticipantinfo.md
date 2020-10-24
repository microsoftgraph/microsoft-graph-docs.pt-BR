---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a642532579d127fdeb48b4c69524975b293ff959
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741996"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="9e601-103">tipo de recurso meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="9e601-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="9e601-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e601-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e601-105">Informações sobre um participante de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="9e601-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="9e601-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e601-106">Properties</span></span>

| <span data-ttu-id="9e601-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e601-107">Property</span></span> | <span data-ttu-id="9e601-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e601-108">Type</span></span>                          | <span data-ttu-id="9e601-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e601-109">Description</span></span>                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| <span data-ttu-id="9e601-110">ladrões</span><span class="sxs-lookup"><span data-stu-id="9e601-110">identity</span></span> | [<span data-ttu-id="9e601-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="9e601-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="9e601-112">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="9e601-112">Identity information of the participant.</span></span>                                            |
| <span data-ttu-id="9e601-113">UPN</span><span class="sxs-lookup"><span data-stu-id="9e601-113">upn</span></span>      | <span data-ttu-id="9e601-114">String</span><span class="sxs-lookup"><span data-stu-id="9e601-114">String</span></span>                        | <span data-ttu-id="9e601-115">Nome principal do usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="9e601-115">User principal name of the participant.</span></span>                                             |
| <span data-ttu-id="9e601-116">role</span><span class="sxs-lookup"><span data-stu-id="9e601-116">role</span></span>     | <span data-ttu-id="9e601-117">onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="9e601-117">onlineMeetingRole</span></span>             | <span data-ttu-id="9e601-118">Especifica a função do participante na reunião.</span><span class="sxs-lookup"><span data-stu-id="9e601-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="9e601-119">Os valores possíveis estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="9e601-119">Possible values are listed in the following table.</span></span> |

### <a name="onlinemeetingrole-values"></a><span data-ttu-id="9e601-120">valores de onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="9e601-120">onlineMeetingRole values</span></span>

| <span data-ttu-id="9e601-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9e601-121">Value</span></span>              | <span data-ttu-id="9e601-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e601-122">Description</span></span>                     |
| ------------------ | ------------------------------- |
| <span data-ttu-id="9e601-123">attendee</span><span class="sxs-lookup"><span data-stu-id="9e601-123">attendee</span></span>           | <span data-ttu-id="9e601-124">O participante é um participante.</span><span class="sxs-lookup"><span data-stu-id="9e601-124">The participant is an attendee.</span></span> |
| <span data-ttu-id="9e601-125">instrutor</span><span class="sxs-lookup"><span data-stu-id="9e601-125">presenter</span></span>          | <span data-ttu-id="9e601-126">O participante é um apresentador.</span><span class="sxs-lookup"><span data-stu-id="9e601-126">The participant is a presenter.</span></span> |
| <span data-ttu-id="9e601-127">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="9e601-127">unknownFutureValue</span></span> | <span data-ttu-id="9e601-128">Valor de futuro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="9e601-128">Unknown future value.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="9e601-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e601-129">JSON representation</span></span>

<span data-ttu-id="9e601-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e601-130">The following is a JSON representation of the resource.</span></span>

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

