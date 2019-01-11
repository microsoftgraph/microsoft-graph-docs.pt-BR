---
title: tipo de recurso de invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associado a um convite para conversa e fornece os parâmetros adicionais de convite.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 7a6fb418b7076b0f0a42dc05b6afe71dcda6a71e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864999"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="385f9-103">tipo de recurso de invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="385f9-103">invitationParticipantInfo resource type</span></span>

> <span data-ttu-id="385f9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="385f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="385f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="385f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="385f9-106">O **InvitationParticipant** é usado para representar um conjunto de identidades associado a um convite para conversa e fornece os parâmetros adicionais de convite.</span><span class="sxs-lookup"><span data-stu-id="385f9-106">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="385f9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="385f9-107">Properties</span></span>

| <span data-ttu-id="385f9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="385f9-108">Property</span></span>                           | <span data-ttu-id="385f9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="385f9-109">Type</span></span>                          | <span data-ttu-id="385f9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="385f9-110">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="385f9-111">endpointType</span><span class="sxs-lookup"><span data-stu-id="385f9-111">endpointType</span></span>                       | <span data-ttu-id="385f9-112">String</span><span class="sxs-lookup"><span data-stu-id="385f9-112">String</span></span>                        | <span data-ttu-id="385f9-113">Os valores possíveis são: `default` e `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="385f9-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="385f9-114">identity</span><span class="sxs-lookup"><span data-stu-id="385f9-114">identity</span></span>                           | [<span data-ttu-id="385f9-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="385f9-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="385f9-116">O [identitySet](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="385f9-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="385f9-117">languageId</span><span class="sxs-lookup"><span data-stu-id="385f9-117">languageId</span></span>                         | <span data-ttu-id="385f9-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="385f9-118">String</span></span>                        | <span data-ttu-id="385f9-119">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="385f9-119">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="385f9-120">região</span><span class="sxs-lookup"><span data-stu-id="385f9-120">region</span></span>                             | <span data-ttu-id="385f9-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="385f9-121">String</span></span>                        | <span data-ttu-id="385f9-122">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="385f9-122">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="385f9-123">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="385f9-123">replacesCallId</span></span>                     | <span data-ttu-id="385f9-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="385f9-124">String</span></span>                        | <span data-ttu-id="385f9-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="385f9-125">Optional.</span></span> <span data-ttu-id="385f9-126">A chamada que o idenity de destino no momento é parte do.</span><span class="sxs-lookup"><span data-stu-id="385f9-126">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="385f9-127">Essa chamada será descartada depois que o participante é adicionado.</span><span class="sxs-lookup"><span data-stu-id="385f9-127">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="385f9-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="385f9-128">JSON representation</span></span>

<span data-ttu-id="385f9-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="385f9-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
