---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0df39f5fb94f648e8d5c5a8b0ff9a10c7a9a7efa
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939282"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="cf2fc-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="cf2fc-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf2fc-104">Configurações da caixa de correio principal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="cf2fc-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="cf2fc-105">Você pode [obter](../api/user-get-mailboxsettings.md) ou [Atualizar](../api/user-update-mailboxsettings.md) as configurações de caixa de correio de um usuário consultando a propriedade **mailboxSettings** do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="cf2fc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf2fc-106">Properties</span></span>
| <span data-ttu-id="cf2fc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf2fc-107">Property</span></span>     | <span data-ttu-id="cf2fc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf2fc-108">Type</span></span>   |<span data-ttu-id="cf2fc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf2fc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf2fc-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="cf2fc-110">archiveFolder</span></span>|<span data-ttu-id="cf2fc-111">string</span><span class="sxs-lookup"><span data-stu-id="cf2fc-111">string</span></span>|<span data-ttu-id="cf2fc-112">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="cf2fc-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="cf2fc-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="cf2fc-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="cf2fc-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="cf2fc-115">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="cf2fc-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="cf2fc-116">dateFormat</span></span>|<span data-ttu-id="cf2fc-117">string</span><span class="sxs-lookup"><span data-stu-id="cf2fc-117">string</span></span>|<span data-ttu-id="cf2fc-118">O formato de data da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="cf2fc-119">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="cf2fc-119">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="cf2fc-120">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="cf2fc-120">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="cf2fc-121">Se o usuário tiver um representante de calendário, isso especificará se o representante, o proprietário da caixa de correio ou ambos recebem mensagens de reunião e respostas da reunião.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-121">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="cf2fc-122">Os valores possíveis são: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-122">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="cf2fc-123">idioma</span><span class="sxs-lookup"><span data-stu-id="cf2fc-123">language</span></span>|[<span data-ttu-id="cf2fc-124">localeInfo</span><span class="sxs-lookup"><span data-stu-id="cf2fc-124">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="cf2fc-125">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-125">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="cf2fc-126">Formato de TimeFormat</span><span class="sxs-lookup"><span data-stu-id="cf2fc-126">timeFormat</span></span>|<span data-ttu-id="cf2fc-127">string</span><span class="sxs-lookup"><span data-stu-id="cf2fc-127">string</span></span>|<span data-ttu-id="cf2fc-128">O formato de hora da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-128">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="cf2fc-129">timeZone</span><span class="sxs-lookup"><span data-stu-id="cf2fc-129">timeZone</span></span>|<span data-ttu-id="cf2fc-130">string</span><span class="sxs-lookup"><span data-stu-id="cf2fc-130">string</span></span>|<span data-ttu-id="cf2fc-131">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-131">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="cf2fc-132">workingHours</span><span class="sxs-lookup"><span data-stu-id="cf2fc-132">workingHours</span></span>|[<span data-ttu-id="cf2fc-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="cf2fc-133">workingHours</span></span>](workinghours.md)|<span data-ttu-id="cf2fc-134">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-134">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf2fc-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf2fc-135">JSON representation</span></span>

<span data-ttu-id="cf2fc-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "dateFormat": "string",
  "delegateMeetingMessageDeliveryOptions": "String",
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeFormat": "string",
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
