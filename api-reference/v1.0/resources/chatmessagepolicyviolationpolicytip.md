---
title: tipo de recurso chatMessagePolicyViolationPolicyTip
description: Representa as propriedades de uma dica de política em um objeto chatMessagePolicyViolation. As dicas de política fornecem ao remetente informações sobre a violação da política.
author: laujan
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ccc3680f5b0365e1f54e9b82743b6906750b272
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223929"
---
# <a name="chatmessagepolicytip-resource-type"></a><span data-ttu-id="f24fb-104">tipo de recurso chatMessagePolicyTip</span><span class="sxs-lookup"><span data-stu-id="f24fb-104">chatMessagePolicyTip resource type</span></span>

<span data-ttu-id="f24fb-105">Representa as propriedades de uma dica de política em um objeto [chatMessagePolicyViolation](chatmessagepolicyviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="f24fb-105">Represents the properties of a policy tip on a [chatMessagePolicyViolation](chatmessagepolicyviolation.md) object.</span></span> <span data-ttu-id="f24fb-106">As dicas de política fornecem ao remetente informações sobre a violação da política.</span><span class="sxs-lookup"><span data-stu-id="f24fb-106">Policy tips provide the sender with information about the policy violation.</span></span>
<span data-ttu-id="f24fb-107">As dicas de política são normalmente definidas por um aplicativo DLP (prevenção de perda de dados) que observa mensagens que contêm dados que os usuários não devem enviar.</span><span class="sxs-lookup"><span data-stu-id="f24fb-107">Policy tips are typically set by a data loss prevention (DLP) app which watches for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="f24fb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f24fb-108">Properties</span></span>

| <span data-ttu-id="f24fb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f24fb-109">Property</span></span>   | <span data-ttu-id="f24fb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f24fb-110">Type</span></span> |<span data-ttu-id="f24fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f24fb-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f24fb-112">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="f24fb-112">complianceUrl</span></span>|<span data-ttu-id="f24fb-113">string</span><span class="sxs-lookup"><span data-stu-id="f24fb-113">string</span></span>|<span data-ttu-id="f24fb-114">A URL que um usuário pode visitar para ler sobre as políticas de prevenção de perda de dados da organização.</span><span class="sxs-lookup"><span data-stu-id="f24fb-114">The URL a user can visit to read about the data loss prevention policies for the organization.</span></span> <span data-ttu-id="f24fb-115">(IE, políticas sobre o que os usuários não devem dizer nos chats)</span><span class="sxs-lookup"><span data-stu-id="f24fb-115">(ie, policies about what users shouldn't say in chats)</span></span>|
|<span data-ttu-id="f24fb-116">generalText</span><span class="sxs-lookup"><span data-stu-id="f24fb-116">generalText</span></span>|<span data-ttu-id="f24fb-117">string</span><span class="sxs-lookup"><span data-stu-id="f24fb-117">string</span></span>|<span data-ttu-id="f24fb-118">Texto explicativo mostrado ao remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="f24fb-118">Explanatory text shown to the sender of the message.</span></span>|
|<span data-ttu-id="f24fb-119">matchedConditionDescriptions</span><span class="sxs-lookup"><span data-stu-id="f24fb-119">matchedConditionDescriptions</span></span>|<span data-ttu-id="f24fb-120">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f24fb-120">string collection</span></span>|<span data-ttu-id="f24fb-121">A lista de dados inadequados na mensagem que foi detectada pelo aplicativo prevenção de perda de dados.</span><span class="sxs-lookup"><span data-stu-id="f24fb-121">The list of improper data in the message that was detected by the data loss prevention app.</span></span> <span data-ttu-id="f24fb-122">Cada aplicativo DLP define suas próprias condições, exemplos incluem "número do cartão de crédito" e "número do CPF".</span><span class="sxs-lookup"><span data-stu-id="f24fb-122">Each DLP app defines its own conditions, examples include "Credit Card Number" and "Social Security Number".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f24fb-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f24fb-123">JSON representation</span></span>

<span data-ttu-id="f24fb-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f24fb-124">The following is a JSON representation of the resource.</span></span>

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
