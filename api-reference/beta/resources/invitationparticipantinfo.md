---
title: tipo de recurso de invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associado a um convite para conversa e fornece os parâmetros adicionais de convite.
author: VinodRavichandran
ms.openlocfilehash: f833fcd0c555dfcc88da4027313ed7f40da81428
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380482"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="37dc1-103">tipo de recurso de invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="37dc1-103">invitationParticipantInfo resource type</span></span>

> <span data-ttu-id="37dc1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="37dc1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37dc1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="37dc1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37dc1-106">O **InvitationParticipant** é usado para representar um conjunto de identidades associado a um convite para conversa e fornece os parâmetros adicionais de convite.</span><span class="sxs-lookup"><span data-stu-id="37dc1-106">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="37dc1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37dc1-107">Properties</span></span>

| <span data-ttu-id="37dc1-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="37dc1-108">Property</span></span>                           | <span data-ttu-id="37dc1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="37dc1-109">Type</span></span>                          | <span data-ttu-id="37dc1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="37dc1-110">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="37dc1-111">endpointType</span><span class="sxs-lookup"><span data-stu-id="37dc1-111">endpointType</span></span>                       | <span data-ttu-id="37dc1-112">String</span><span class="sxs-lookup"><span data-stu-id="37dc1-112">String</span></span>                        | <span data-ttu-id="37dc1-113">Os valores possíveis são: `default` e `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="37dc1-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="37dc1-114">identity</span><span class="sxs-lookup"><span data-stu-id="37dc1-114">identity</span></span>                           | [<span data-ttu-id="37dc1-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="37dc1-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="37dc1-116">O [identitySet](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="37dc1-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="37dc1-117">languageId</span><span class="sxs-lookup"><span data-stu-id="37dc1-117">languageId</span></span>                         | <span data-ttu-id="37dc1-118">String</span><span class="sxs-lookup"><span data-stu-id="37dc1-118">String</span></span>                        | <span data-ttu-id="37dc1-119">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="37dc1-119">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="37dc1-120">região</span><span class="sxs-lookup"><span data-stu-id="37dc1-120">region</span></span>                             | <span data-ttu-id="37dc1-121">String</span><span class="sxs-lookup"><span data-stu-id="37dc1-121">String</span></span>                        | <span data-ttu-id="37dc1-122">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="37dc1-122">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="37dc1-123">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="37dc1-123">replacesCallId</span></span>                     | <span data-ttu-id="37dc1-124">String</span><span class="sxs-lookup"><span data-stu-id="37dc1-124">String</span></span>                        | <span data-ttu-id="37dc1-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37dc1-125">Optional.</span></span> <span data-ttu-id="37dc1-126">A chamada que o idenity de destino no momento é parte do.</span><span class="sxs-lookup"><span data-stu-id="37dc1-126">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="37dc1-127">Essa chamada será descartada depois que o participante é adicionado.</span><span class="sxs-lookup"><span data-stu-id="37dc1-127">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37dc1-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37dc1-128">JSON representation</span></span>

<span data-ttu-id="37dc1-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37dc1-129">The following is a JSON representation of the resource.</span></span>

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
