---
title: Tipo de recurso automaticRepliesSetting
description: 'Definições de configuração para notificar automaticamente o remetente de um email de entrada com uma mensagem da '
localization_priority: Normal
ms.openlocfilehash: 81fb16a9124c60f43887150917f132579aa4f163
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569421"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="b6c5c-103">Tipo de recurso automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b6c5c-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="b6c5c-p101">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Por exemplo, uma resposta automática para notificar que o usuário conectado está disponível para responder a emails.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="b6c5c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6c5c-106">Properties</span></span>
| <span data-ttu-id="b6c5c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6c5c-107">Property</span></span>     | <span data-ttu-id="b6c5c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6c5c-108">Type</span></span>   |<span data-ttu-id="b6c5c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6c5c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6c5c-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="b6c5c-110">externalAudience</span></span>|<span data-ttu-id="b6c5c-111">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="b6c5c-111">externalAudienceScope</span></span>| <span data-ttu-id="b6c5c-112">O conjunto da audiência externa para a organização do usuário conectado que receberá **ExternalReplyMessage**, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-112">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> <span data-ttu-id="b6c5c-113">Os valores possíveis são: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-113">The possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="b6c5c-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="b6c5c-114">externalReplyMessage</span></span>|<span data-ttu-id="b6c5c-115">string</span><span class="sxs-lookup"><span data-stu-id="b6c5c-115">string</span></span>|<span data-ttu-id="b6c5c-116">A resposta automática para enviar à audiência externa especificada, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="b6c5c-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="b6c5c-117">internalReplyMessage</span></span>|<span data-ttu-id="b6c5c-118">string</span><span class="sxs-lookup"><span data-stu-id="b6c5c-118">string</span></span>|<span data-ttu-id="b6c5c-119">A resposta automática para enviar à audiência interna na organização do usuário conectado, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="b6c5c-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="b6c5c-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="b6c5c-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b6c5c-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b6c5c-122">A data e a hora em que as respostas automáticas estão definidas para terminar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="b6c5c-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="b6c5c-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="b6c5c-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b6c5c-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b6c5c-125">A data e a hora em que as respostas automáticas estão definidas para começar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="b6c5c-126">status</span><span class="sxs-lookup"><span data-stu-id="b6c5c-126">status</span></span>|<span data-ttu-id="b6c5c-127">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="b6c5c-127">automaticRepliesStatus</span></span>|<span data-ttu-id="b6c5c-128">Status de configurações de respostas automáticas.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-128">Configurations status for automatic replies.</span></span> <span data-ttu-id="b6c5c-129">Os valores possíveis são: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-129">The possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6c5c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6c5c-130">JSON representation</span></span>

<span data-ttu-id="b6c5c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6c5c-131">Here is a JSON representation of the resource.</span></span>

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
