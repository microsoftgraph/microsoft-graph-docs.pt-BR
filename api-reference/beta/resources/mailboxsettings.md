---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6d966ecb599d98c92bf1e70eca1f61fb665e359d
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652041"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="c74d3-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="c74d3-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c74d3-104">Configurações da caixa de correio principal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="c74d3-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="c74d3-105">Você pode [obter](../api/user-get-mailboxsettings.md) ou [Atualizar](../api/user-update-mailboxsettings.md) as configurações de caixa de correio de um usuário consultando a propriedade **mailboxSettings** do usuário.</span><span class="sxs-lookup"><span data-stu-id="c74d3-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="c74d3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c74d3-106">Properties</span></span>
| <span data-ttu-id="c74d3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c74d3-107">Property</span></span>     | <span data-ttu-id="c74d3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c74d3-108">Type</span></span>   |<span data-ttu-id="c74d3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c74d3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c74d3-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="c74d3-110">archiveFolder</span></span>|<span data-ttu-id="c74d3-111">string</span><span class="sxs-lookup"><span data-stu-id="c74d3-111">string</span></span>|<span data-ttu-id="c74d3-112">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="c74d3-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="c74d3-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="c74d3-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="c74d3-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="c74d3-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="c74d3-115">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="c74d3-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="c74d3-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="c74d3-116">dateFormat</span></span>|<span data-ttu-id="c74d3-117">string</span><span class="sxs-lookup"><span data-stu-id="c74d3-117">string</span></span>|<span data-ttu-id="c74d3-118">O formato de data da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="c74d3-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="c74d3-119">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="c74d3-119">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="c74d3-120">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="c74d3-120">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="c74d3-121">Se o usuário tiver um representante de calendário, isso especificará se o representante, o proprietário da caixa de correio ou ambos recebem mensagens de reunião e respostas da reunião.</span><span class="sxs-lookup"><span data-stu-id="c74d3-121">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="c74d3-122">Os valores possíveis são: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="c74d3-122">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span> <span data-ttu-id="c74d3-123">O padrão é `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="c74d3-123">The default is `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="c74d3-124">idioma</span><span class="sxs-lookup"><span data-stu-id="c74d3-124">language</span></span>|[<span data-ttu-id="c74d3-125">localeInfo</span><span class="sxs-lookup"><span data-stu-id="c74d3-125">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="c74d3-126">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="c74d3-126">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="c74d3-127">Formato de TimeFormat</span><span class="sxs-lookup"><span data-stu-id="c74d3-127">timeFormat</span></span>|<span data-ttu-id="c74d3-128">string</span><span class="sxs-lookup"><span data-stu-id="c74d3-128">string</span></span>|<span data-ttu-id="c74d3-129">O formato de hora da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="c74d3-129">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="c74d3-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="c74d3-130">timeZone</span></span>|<span data-ttu-id="c74d3-131">string</span><span class="sxs-lookup"><span data-stu-id="c74d3-131">string</span></span>|<span data-ttu-id="c74d3-132">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="c74d3-132">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="c74d3-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="c74d3-133">workingHours</span></span>|[<span data-ttu-id="c74d3-134">workingHours</span><span class="sxs-lookup"><span data-stu-id="c74d3-134">workingHours</span></span>](workinghours.md)|<span data-ttu-id="c74d3-135">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="c74d3-135">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c74d3-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c74d3-136">JSON representation</span></span>

<span data-ttu-id="c74d3-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c74d3-137">Here is a JSON representation of the resource.</span></span>

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
