---
title: Tipo de recurso chatMessagePolicyViolationPolicyTip
description: Representa propriedades de uma dica de política em um objeto chatMessagePolicyViolation. As dicas de política fornecem ao remetente informações sobre a violação da política.
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 58b0a80a7e9a8864b13e36e2cef8355c46fd340d
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582741"
---
# <a name="chatmessagepolicytip-resource-type"></a><span data-ttu-id="effdf-104">Tipo de recurso chatMessagePolicyTip</span><span class="sxs-lookup"><span data-stu-id="effdf-104">chatMessagePolicyTip resource type</span></span>

<span data-ttu-id="effdf-105">Representa as propriedades de uma dica de política em um [objeto chatMessagePolicyViolation.](chatmessagepolicyviolation.md)</span><span class="sxs-lookup"><span data-stu-id="effdf-105">Represents the properties of a policy tip on a [chatMessagePolicyViolation](chatmessagepolicyviolation.md) object.</span></span> <span data-ttu-id="effdf-106">As dicas de política fornecem ao remetente informações sobre a violação da política.</span><span class="sxs-lookup"><span data-stu-id="effdf-106">Policy tips provide the sender with information about the policy violation.</span></span>
<span data-ttu-id="effdf-107">As dicas de política geralmente são definidas por um aplicativo de prevenção contra perda de dados (DLP) que observa mensagens que contêm dados que os usuários não devem enviar.</span><span class="sxs-lookup"><span data-stu-id="effdf-107">Policy tips are typically set by a data loss prevention (DLP) app which watches for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="effdf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="effdf-108">Properties</span></span>

| <span data-ttu-id="effdf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="effdf-109">Property</span></span>   | <span data-ttu-id="effdf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="effdf-110">Type</span></span> |<span data-ttu-id="effdf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="effdf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="effdf-112">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="effdf-112">complianceUrl</span></span>|<span data-ttu-id="effdf-113">string</span><span class="sxs-lookup"><span data-stu-id="effdf-113">string</span></span>|<span data-ttu-id="effdf-114">A URL que um usuário pode visitar para ler sobre as políticas de prevenção contra perda de dados da organização.</span><span class="sxs-lookup"><span data-stu-id="effdf-114">The URL a user can visit to read about the data loss prevention policies for the organization.</span></span> <span data-ttu-id="effdf-115">(ou seja, políticas sobre o que os usuários não devem dizer nos chats)</span><span class="sxs-lookup"><span data-stu-id="effdf-115">(ie, policies about what users shouldn't say in chats)</span></span>|
|<span data-ttu-id="effdf-116">generalText</span><span class="sxs-lookup"><span data-stu-id="effdf-116">generalText</span></span>|<span data-ttu-id="effdf-117">string</span><span class="sxs-lookup"><span data-stu-id="effdf-117">string</span></span>|<span data-ttu-id="effdf-118">Texto explicativo mostrado ao remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="effdf-118">Explanatory text shown to the sender of the message.</span></span>|
|<span data-ttu-id="effdf-119">matchedConditionDescriptions</span><span class="sxs-lookup"><span data-stu-id="effdf-119">matchedConditionDescriptions</span></span>|<span data-ttu-id="effdf-120">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="effdf-120">string collection</span></span>|<span data-ttu-id="effdf-121">A lista de dados impróprios na mensagem detectada pelo aplicativo de prevenção contra perda de dados.</span><span class="sxs-lookup"><span data-stu-id="effdf-121">The list of improper data in the message that was detected by the data loss prevention app.</span></span> <span data-ttu-id="effdf-122">Cada aplicativo DLP define suas próprias condições, exemplos incluem "Número do Cartão de Crédito" e "Número da Previdência Social".</span><span class="sxs-lookup"><span data-stu-id="effdf-122">Each DLP app defines its own conditions, examples include "Credit Card Number" and "Social Security Number".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="effdf-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="effdf-123">JSON representation</span></span>

<span data-ttu-id="effdf-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="effdf-124">The following is a JSON representation of the resource.</span></span>

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
