---
title: Tipo de recurso automaticRepliesSetting
description: 'Definições de configuração para notificar automaticamente o remetente de um email de entrada com uma mensagem da '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cad76eb9ebbd8646e96cea1b98cb8d87c20a3b23
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030034"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="2ed47-103">Tipo de recurso automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="2ed47-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="2ed47-p101">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Por exemplo, uma resposta automática para notificar que o usuário conectado está disponível para responder a emails.</span><span class="sxs-lookup"><span data-stu-id="2ed47-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="2ed47-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ed47-106">Properties</span></span>
| <span data-ttu-id="2ed47-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ed47-107">Property</span></span>     | <span data-ttu-id="2ed47-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ed47-108">Type</span></span>   |<span data-ttu-id="2ed47-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ed47-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ed47-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="2ed47-110">externalAudience</span></span>|<span data-ttu-id="2ed47-111">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="2ed47-111">externalAudienceScope</span></span>| <span data-ttu-id="2ed47-112">O conjunto da audiência externa para a organização do usuário conectado que receberá **ExternalReplyMessage**, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="2ed47-112">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> <span data-ttu-id="2ed47-113">Os valores possíveis são: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="2ed47-113">The possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="2ed47-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="2ed47-114">externalReplyMessage</span></span>|<span data-ttu-id="2ed47-115">string</span><span class="sxs-lookup"><span data-stu-id="2ed47-115">string</span></span>|<span data-ttu-id="2ed47-116">A resposta automática para enviar à audiência externa especificada, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="2ed47-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="2ed47-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="2ed47-117">internalReplyMessage</span></span>|<span data-ttu-id="2ed47-118">string</span><span class="sxs-lookup"><span data-stu-id="2ed47-118">string</span></span>|<span data-ttu-id="2ed47-119">A resposta automática para enviar à audiência interna na organização do usuário conectado, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="2ed47-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="2ed47-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="2ed47-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="2ed47-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2ed47-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2ed47-122">A data e a hora em que as respostas automáticas estão definidas para terminar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="2ed47-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="2ed47-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="2ed47-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="2ed47-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2ed47-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2ed47-125">A data e a hora em que as respostas automáticas estão definidas para começar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="2ed47-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="2ed47-126">status</span><span class="sxs-lookup"><span data-stu-id="2ed47-126">status</span></span>|<span data-ttu-id="2ed47-127">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="2ed47-127">automaticRepliesStatus</span></span>|<span data-ttu-id="2ed47-128">Status de configurações de respostas automáticas.</span><span class="sxs-lookup"><span data-stu-id="2ed47-128">Configurations status for automatic replies.</span></span> <span data-ttu-id="2ed47-129">Os valores possíveis são: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="2ed47-129">The possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ed47-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ed47-130">JSON representation</span></span>

<span data-ttu-id="2ed47-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ed47-131">Here is a JSON representation of the resource.</span></span>

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
