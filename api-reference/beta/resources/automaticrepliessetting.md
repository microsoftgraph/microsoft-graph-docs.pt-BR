---
title: Tipo de recurso automaticRepliesSetting
description: 'Definições de configuração automaticamente notificar o remetente de um email de entrada com uma mensagem a partir do '
localization_priority: Normal
ms.openlocfilehash: 0160197a4fafe10b7f78be9124da3b6260bfcee6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820654"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="b95e3-103">Tipo de recurso automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b95e3-103">automaticRepliesSetting resource type</span></span>

> <span data-ttu-id="b95e3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b95e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b95e3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b95e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b95e3-p102">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Por exemplo, uma resposta automática para notificar que o usuário conectado está disponível para responder a emails.</span><span class="sxs-lookup"><span data-stu-id="b95e3-p102">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="b95e3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b95e3-108">Properties</span></span>
| <span data-ttu-id="b95e3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b95e3-109">Property</span></span>     | <span data-ttu-id="b95e3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b95e3-110">Type</span></span>   |<span data-ttu-id="b95e3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b95e3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b95e3-112">externalAudience</span><span class="sxs-lookup"><span data-stu-id="b95e3-112">externalAudience</span></span>|<span data-ttu-id="b95e3-113">String</span><span class="sxs-lookup"><span data-stu-id="b95e3-113">String</span></span>| <span data-ttu-id="b95e3-p103">O conjunto da audiência externa para a organização do usuário conectado que receberá **ExternalReplyMessage**, se **Status** for `AlwaysEnabled` ou `Scheduled`. Os valores possíveis são: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="b95e3-p103">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="b95e3-116">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="b95e3-116">externalReplyMessage</span></span>|<span data-ttu-id="b95e3-117">string</span><span class="sxs-lookup"><span data-stu-id="b95e3-117">string</span></span>|<span data-ttu-id="b95e3-118">A resposta automática para enviar à audiência externa especificada, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b95e3-118">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="b95e3-119">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="b95e3-119">internalReplyMessage</span></span>|<span data-ttu-id="b95e3-120">string</span><span class="sxs-lookup"><span data-stu-id="b95e3-120">string</span></span>|<span data-ttu-id="b95e3-121">A resposta automática para enviar à audiência interna na organização do usuário conectado, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b95e3-121">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="b95e3-122">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="b95e3-122">scheduledEndDateTime</span></span>|[<span data-ttu-id="b95e3-123">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b95e3-123">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b95e3-124">A data e a hora em que as respostas automáticas estão definidas para terminar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b95e3-124">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="b95e3-125">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="b95e3-125">scheduledStartDateTime</span></span>|[<span data-ttu-id="b95e3-126">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b95e3-126">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b95e3-127">A data e a hora em que as respostas automáticas estão definidas para começar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b95e3-127">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="b95e3-128">status</span><span class="sxs-lookup"><span data-stu-id="b95e3-128">status</span></span>|<span data-ttu-id="b95e3-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b95e3-129">String</span></span>|<span data-ttu-id="b95e3-p104">Status de configurações de respostas automáticas. Os valores possíveis são: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b95e3-p104">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b95e3-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b95e3-132">JSON representation</span></span>

<span data-ttu-id="b95e3-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b95e3-133">Here is a JSON representation of the resource.</span></span>

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
