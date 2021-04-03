---
title: Tipo de recurso chatMessagePolicyViolationPolicyTip
description: Representa as propriedades de uma dica de política em um objeto chatMessagePolicyViolation. As dicas de política fornecem ao remetente informações sobre a violação da política.
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c315dbcb37b11e7ed5771544f511c5cf07cc89a8
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582246"
---
# <a name="chatmessagepolicytip-resource-type"></a><span data-ttu-id="fb29b-104">Tipo de recurso chatMessagePolicyTip</span><span class="sxs-lookup"><span data-stu-id="fb29b-104">chatMessagePolicyTip resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb29b-105">Representa as propriedades de uma dica de política em um [objeto chatMessagePolicyViolation.](chatmessagepolicyviolation.md)</span><span class="sxs-lookup"><span data-stu-id="fb29b-105">Represents the properties of a policy tip on a [chatMessagePolicyViolation](chatmessagepolicyviolation.md) object.</span></span> <span data-ttu-id="fb29b-106">As dicas de política fornecem ao remetente informações sobre a violação da política.</span><span class="sxs-lookup"><span data-stu-id="fb29b-106">Policy tips provide the sender with information about the policy violation.</span></span>
<span data-ttu-id="fb29b-107">As dicas de política geralmente são definidas por um aplicativo de prevenção contra perda de dados (DLP) que observa mensagens que contêm dados que os usuários não devem enviar.</span><span class="sxs-lookup"><span data-stu-id="fb29b-107">Policy tips are typically set by a data loss prevention (DLP) app which watches for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="fb29b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb29b-108">Properties</span></span>

| <span data-ttu-id="fb29b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb29b-109">Property</span></span>   | <span data-ttu-id="fb29b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb29b-110">Type</span></span> |<span data-ttu-id="fb29b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb29b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb29b-112">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="fb29b-112">complianceUrl</span></span>|<span data-ttu-id="fb29b-113">string</span><span class="sxs-lookup"><span data-stu-id="fb29b-113">string</span></span>|<span data-ttu-id="fb29b-114">A URL que um usuário pode visitar para ler sobre as políticas de prevenção contra perda de dados da organização.</span><span class="sxs-lookup"><span data-stu-id="fb29b-114">The URL a user can visit to read about the data loss prevention policies for the organization.</span></span> <span data-ttu-id="fb29b-115">(ou seja, políticas sobre o que os usuários não devem dizer nos chats)</span><span class="sxs-lookup"><span data-stu-id="fb29b-115">(ie, policies about what users shouldn't say in chats)</span></span>|
|<span data-ttu-id="fb29b-116">generalText</span><span class="sxs-lookup"><span data-stu-id="fb29b-116">generalText</span></span>|<span data-ttu-id="fb29b-117">string</span><span class="sxs-lookup"><span data-stu-id="fb29b-117">string</span></span>|<span data-ttu-id="fb29b-118">Texto explicativo mostrado ao remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="fb29b-118">Explanatory text shown to the sender of the message.</span></span>|
|<span data-ttu-id="fb29b-119">matchedConditionDescriptions</span><span class="sxs-lookup"><span data-stu-id="fb29b-119">matchedConditionDescriptions</span></span>|<span data-ttu-id="fb29b-120">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb29b-120">string collection</span></span>|<span data-ttu-id="fb29b-121">A lista de dados impróprios na mensagem detectada pelo aplicativo de prevenção contra perda de dados.</span><span class="sxs-lookup"><span data-stu-id="fb29b-121">The list of improper data in the message that was detected by the data loss prevention app.</span></span> <span data-ttu-id="fb29b-122">Cada aplicativo DLP define suas próprias condições, exemplos incluem "Número do Cartão de Crédito" e "Número da Previdência Social".</span><span class="sxs-lookup"><span data-stu-id="fb29b-122">Each DLP app defines its own conditions, examples include "Credit Card Number" and "Social Security Number".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb29b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb29b-123">JSON representation</span></span>

<span data-ttu-id="fb29b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb29b-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "generalText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"
}-->
```json
{
  "complianceUrl": "string",
  "generalText": "string",
  "matchedConditionDescriptions": ["string 1", "string 2"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policy violation policy tip resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
