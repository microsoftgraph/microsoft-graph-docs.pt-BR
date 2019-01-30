---
title: Tipo de recurso automaticRepliesSetting
description: 'Definições de configuração automaticamente notificar o remetente de um email de entrada com uma mensagem a partir do '
localization_priority: Normal
ms.openlocfilehash: 5ff16aa93042e0d66063cb62de7a8dcdf870c892
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641250"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="9f47f-103">Tipo de recurso automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="9f47f-103">automaticRepliesSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f47f-p101">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Por exemplo, uma resposta automática para notificar que o usuário conectado está disponível para responder a emails.</span><span class="sxs-lookup"><span data-stu-id="9f47f-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="9f47f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f47f-106">Properties</span></span>
| <span data-ttu-id="9f47f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f47f-107">Property</span></span>     | <span data-ttu-id="9f47f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f47f-108">Type</span></span>   |<span data-ttu-id="9f47f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f47f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f47f-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="9f47f-110">externalAudience</span></span>|<span data-ttu-id="9f47f-111">String</span><span class="sxs-lookup"><span data-stu-id="9f47f-111">String</span></span>| <span data-ttu-id="9f47f-p102">O conjunto da audiência externa para a organização do usuário conectado que receberá **ExternalReplyMessage**, se **Status** for `AlwaysEnabled` ou `Scheduled`. Os valores possíveis são: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="9f47f-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="9f47f-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="9f47f-114">externalReplyMessage</span></span>|<span data-ttu-id="9f47f-115">string</span><span class="sxs-lookup"><span data-stu-id="9f47f-115">string</span></span>|<span data-ttu-id="9f47f-116">A resposta automática para enviar à audiência externa especificada, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="9f47f-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="9f47f-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="9f47f-117">internalReplyMessage</span></span>|<span data-ttu-id="9f47f-118">string</span><span class="sxs-lookup"><span data-stu-id="9f47f-118">string</span></span>|<span data-ttu-id="9f47f-119">A resposta automática para enviar à audiência interna na organização do usuário conectado, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="9f47f-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="9f47f-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="9f47f-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="9f47f-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9f47f-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9f47f-122">A data e a hora em que as respostas automáticas estão definidas para terminar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="9f47f-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="9f47f-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9f47f-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="9f47f-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9f47f-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9f47f-125">A data e a hora em que as respostas automáticas estão definidas para começar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="9f47f-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="9f47f-126">status</span><span class="sxs-lookup"><span data-stu-id="9f47f-126">status</span></span>|<span data-ttu-id="9f47f-127">String</span><span class="sxs-lookup"><span data-stu-id="9f47f-127">String</span></span>|<span data-ttu-id="9f47f-p103">Status de configurações de respostas automáticas. Os valores possíveis são: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="9f47f-p103">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f47f-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f47f-130">JSON representation</span></span>

<span data-ttu-id="9f47f-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f47f-131">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliessetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
