---
title: Tipo de recurso automaticRepliesSetting
description: 'Definições de configuração para notificar automaticamente o remetente de um email de entrada com uma mensagem da '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 219899ce529c573b3c1d2cb6194d2349979f28d3
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811543"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="e2ccd-103">Tipo de recurso automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="e2ccd-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="e2ccd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2ccd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2ccd-p101">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Por exemplo, uma resposta automática para notificar que o usuário conectado está disponível para responder a emails.</span><span class="sxs-lookup"><span data-stu-id="e2ccd-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span>


## <a name="properties"></a><span data-ttu-id="e2ccd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2ccd-107">Properties</span></span>
| <span data-ttu-id="e2ccd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2ccd-108">Property</span></span>     | <span data-ttu-id="e2ccd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2ccd-109">Type</span></span>   |<span data-ttu-id="e2ccd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2ccd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2ccd-111">externalAudience</span><span class="sxs-lookup"><span data-stu-id="e2ccd-111">externalAudience</span></span>|<span data-ttu-id="e2ccd-112">String</span><span class="sxs-lookup"><span data-stu-id="e2ccd-112">String</span></span>| <span data-ttu-id="e2ccd-p102">O conjunto da audiência externa para a organização do usuário conectado que receberá **ExternalReplyMessage**, se **Status** for `AlwaysEnabled` ou `Scheduled`. Os valores possíveis são: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="e2ccd-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="e2ccd-115">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="e2ccd-115">externalReplyMessage</span></span>|<span data-ttu-id="e2ccd-116">string</span><span class="sxs-lookup"><span data-stu-id="e2ccd-116">string</span></span>|<span data-ttu-id="e2ccd-117">A resposta automática para enviar à audiência externa especificada, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="e2ccd-117">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="e2ccd-118">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="e2ccd-118">internalReplyMessage</span></span>|<span data-ttu-id="e2ccd-119">string</span><span class="sxs-lookup"><span data-stu-id="e2ccd-119">string</span></span>|<span data-ttu-id="e2ccd-120">A resposta automática para enviar à audiência interna na organização do usuário conectado, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="e2ccd-120">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="e2ccd-121">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="e2ccd-121">scheduledEndDateTime</span></span>|[<span data-ttu-id="e2ccd-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e2ccd-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e2ccd-123">A data e a hora em que as respostas automáticas estão definidas para terminar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="e2ccd-123">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="e2ccd-124">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="e2ccd-124">scheduledStartDateTime</span></span>|[<span data-ttu-id="e2ccd-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e2ccd-125">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e2ccd-126">A data e a hora em que as respostas automáticas estão definidas para começar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="e2ccd-126">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="e2ccd-127">status</span><span class="sxs-lookup"><span data-stu-id="e2ccd-127">status</span></span>|<span data-ttu-id="e2ccd-128">String</span><span class="sxs-lookup"><span data-stu-id="e2ccd-128">String</span></span>|<span data-ttu-id="e2ccd-p103">Status de configurações de respostas automáticas. Os valores possíveis são: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="e2ccd-p103">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2ccd-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2ccd-131">JSON representation</span></span>

<span data-ttu-id="e2ccd-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2ccd-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
