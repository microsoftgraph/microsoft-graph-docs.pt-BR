---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c2fb1cb6f45b91843b7c57aa66f6c136d24db2c2
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229049"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="53691-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="53691-103">mailboxSettings resource type</span></span>

<span data-ttu-id="53691-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53691-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53691-105">Configurações da caixa de correio principal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="53691-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="53691-106">Você pode [obter](../api/user-get-mailboxsettings.md) ou [Atualizar](../api/user-update-mailboxsettings.md) as configurações de caixa de correio de um usuário consultando a propriedade **mailboxSettings** do usuário.</span><span class="sxs-lookup"><span data-stu-id="53691-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="53691-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53691-107">Properties</span></span>
| <span data-ttu-id="53691-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53691-108">Property</span></span>     | <span data-ttu-id="53691-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="53691-109">Type</span></span>   |<span data-ttu-id="53691-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="53691-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53691-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="53691-111">archiveFolder</span></span>|<span data-ttu-id="53691-112">string</span><span class="sxs-lookup"><span data-stu-id="53691-112">string</span></span>|<span data-ttu-id="53691-113">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="53691-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="53691-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="53691-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="53691-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="53691-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="53691-116">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="53691-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="53691-117">dateFormat</span><span class="sxs-lookup"><span data-stu-id="53691-117">dateFormat</span></span>|<span data-ttu-id="53691-118">string</span><span class="sxs-lookup"><span data-stu-id="53691-118">string</span></span>|<span data-ttu-id="53691-119">O formato de data da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="53691-119">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="53691-120">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="53691-120">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="53691-121">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="53691-121">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="53691-122">Se o usuário tiver um representante de calendário, isso especificará se o representante, o proprietário da caixa de correio ou ambos recebem mensagens de reunião e respostas da reunião.</span><span class="sxs-lookup"><span data-stu-id="53691-122">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="53691-123">Os valores possíveis são: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="53691-123">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="53691-124">idioma</span><span class="sxs-lookup"><span data-stu-id="53691-124">language</span></span>|[<span data-ttu-id="53691-125">localeInfo</span><span class="sxs-lookup"><span data-stu-id="53691-125">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="53691-126">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="53691-126">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="53691-127">Formato de TimeFormat</span><span class="sxs-lookup"><span data-stu-id="53691-127">timeFormat</span></span>|<span data-ttu-id="53691-128">string</span><span class="sxs-lookup"><span data-stu-id="53691-128">string</span></span>|<span data-ttu-id="53691-129">O formato de hora da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="53691-129">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="53691-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="53691-130">timeZone</span></span>|<span data-ttu-id="53691-131">string</span><span class="sxs-lookup"><span data-stu-id="53691-131">string</span></span>|<span data-ttu-id="53691-132">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="53691-132">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="53691-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="53691-133">workingHours</span></span>|[<span data-ttu-id="53691-134">workingHours</span><span class="sxs-lookup"><span data-stu-id="53691-134">workingHours</span></span>](workinghours.md)|<span data-ttu-id="53691-135">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="53691-135">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53691-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53691-136">JSON representation</span></span>

<span data-ttu-id="53691-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53691-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
