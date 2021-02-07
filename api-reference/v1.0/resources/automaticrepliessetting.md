---
title: Tipo de recurso automaticRepliesSetting
description: 'Definições de configuração para notificar automaticamente o remetente de um email de entrada com uma mensagem do '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 89329e195c47177dc7297a636b53f16ea8d93be4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132392"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="6dc38-103">Tipo de recurso automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="6dc38-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="6dc38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dc38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6dc38-p101">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Por exemplo, uma resposta automática para notificar que o usuário conectado está disponível para responder a emails.</span><span class="sxs-lookup"><span data-stu-id="6dc38-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span>


## <a name="properties"></a><span data-ttu-id="6dc38-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6dc38-107">Properties</span></span>
| <span data-ttu-id="6dc38-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dc38-108">Property</span></span>     | <span data-ttu-id="6dc38-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dc38-109">Type</span></span>   |<span data-ttu-id="6dc38-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc38-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dc38-111">externalAudience</span><span class="sxs-lookup"><span data-stu-id="6dc38-111">externalAudience</span></span>|<span data-ttu-id="6dc38-112">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="6dc38-112">externalAudienceScope</span></span>| <span data-ttu-id="6dc38-113">O conjunto da audiência externa para a organização do usuário conectado que receberá **ExternalReplyMessage**, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="6dc38-113">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> <span data-ttu-id="6dc38-114">Os valores possíveis são: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="6dc38-114">The possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="6dc38-115">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="6dc38-115">externalReplyMessage</span></span>|<span data-ttu-id="6dc38-116">string</span><span class="sxs-lookup"><span data-stu-id="6dc38-116">string</span></span>|<span data-ttu-id="6dc38-117">A resposta automática para enviar à audiência externa especificada, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="6dc38-117">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="6dc38-118">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="6dc38-118">internalReplyMessage</span></span>|<span data-ttu-id="6dc38-119">string</span><span class="sxs-lookup"><span data-stu-id="6dc38-119">string</span></span>|<span data-ttu-id="6dc38-120">A resposta automática para enviar à audiência interna na organização do usuário conectado, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="6dc38-120">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="6dc38-121">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc38-121">scheduledEndDateTime</span></span>|[<span data-ttu-id="6dc38-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6dc38-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6dc38-123">A data e a hora em que as respostas automáticas estão definidas para terminar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="6dc38-123">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="6dc38-124">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc38-124">scheduledStartDateTime</span></span>|[<span data-ttu-id="6dc38-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6dc38-125">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6dc38-126">A data e a hora em que as respostas automáticas estão definidas para começar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="6dc38-126">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="6dc38-127">status</span><span class="sxs-lookup"><span data-stu-id="6dc38-127">status</span></span>|<span data-ttu-id="6dc38-128">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="6dc38-128">automaticRepliesStatus</span></span>|<span data-ttu-id="6dc38-129">Status de configurações de respostas automáticas.</span><span class="sxs-lookup"><span data-stu-id="6dc38-129">Configurations status for automatic replies.</span></span> <span data-ttu-id="6dc38-130">Os valores possíveis são: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="6dc38-130">The possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6dc38-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6dc38-131">JSON representation</span></span>

<span data-ttu-id="6dc38-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6dc38-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

