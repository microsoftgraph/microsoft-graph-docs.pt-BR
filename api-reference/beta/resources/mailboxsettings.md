---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 36cc855b76b7d87d951f733fd0f84739f04aa138
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846167"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="48377-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="48377-103">mailboxSettings resource type</span></span>

<span data-ttu-id="48377-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48377-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48377-105">Configurações da caixa de correio principal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="48377-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="48377-106">Você pode [obter](../api/user-get-mailboxsettings.md) ou [Atualizar](../api/user-update-mailboxsettings.md) as configurações de caixa de correio de um usuário consultando a propriedade **mailboxSettings** do usuário.</span><span class="sxs-lookup"><span data-stu-id="48377-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="48377-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48377-107">Properties</span></span>
| <span data-ttu-id="48377-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48377-108">Property</span></span>     | <span data-ttu-id="48377-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="48377-109">Type</span></span>   |<span data-ttu-id="48377-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="48377-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48377-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="48377-111">archiveFolder</span></span>|<span data-ttu-id="48377-112">string</span><span class="sxs-lookup"><span data-stu-id="48377-112">string</span></span>|<span data-ttu-id="48377-113">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="48377-113">Folder ID of an archive folder for the user.</span></span> <span data-ttu-id="48377-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="48377-114">Read only.</span></span>|
|<span data-ttu-id="48377-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="48377-115">automaticRepliesSetting</span></span>|[<span data-ttu-id="48377-116">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="48377-116">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="48377-117">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="48377-117">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="48377-118">dateFormat</span><span class="sxs-lookup"><span data-stu-id="48377-118">dateFormat</span></span>|<span data-ttu-id="48377-119">string</span><span class="sxs-lookup"><span data-stu-id="48377-119">string</span></span>|<span data-ttu-id="48377-120">O formato de data da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="48377-120">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="48377-121">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="48377-121">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="48377-122">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="48377-122">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="48377-123">Se o usuário tiver um representante de calendário, isso especificará se o representante, o proprietário da caixa de correio ou ambos recebem mensagens de reunião e respostas da reunião.</span><span class="sxs-lookup"><span data-stu-id="48377-123">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="48377-124">Os valores possíveis são: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="48377-124">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span> <span data-ttu-id="48377-125">O padrão é `sendToDelegateOnly` .</span><span class="sxs-lookup"><span data-stu-id="48377-125">The default is `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="48377-126">idioma</span><span class="sxs-lookup"><span data-stu-id="48377-126">language</span></span>|[<span data-ttu-id="48377-127">localeInfo</span><span class="sxs-lookup"><span data-stu-id="48377-127">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="48377-128">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="48377-128">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="48377-129">Formato de TimeFormat</span><span class="sxs-lookup"><span data-stu-id="48377-129">timeFormat</span></span>|<span data-ttu-id="48377-130">string</span><span class="sxs-lookup"><span data-stu-id="48377-130">string</span></span>|<span data-ttu-id="48377-131">O formato de hora da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="48377-131">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="48377-132">timeZone</span><span class="sxs-lookup"><span data-stu-id="48377-132">timeZone</span></span>|<span data-ttu-id="48377-133">string</span><span class="sxs-lookup"><span data-stu-id="48377-133">string</span></span>|<span data-ttu-id="48377-134">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="48377-134">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="48377-135">workingHours</span><span class="sxs-lookup"><span data-stu-id="48377-135">workingHours</span></span>|[<span data-ttu-id="48377-136">workingHours</span><span class="sxs-lookup"><span data-stu-id="48377-136">workingHours</span></span>](workinghours.md)|<span data-ttu-id="48377-137">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="48377-137">The days of the week and hours in a specific time zone that the user works.</span></span>|
|<span data-ttu-id="48377-138">userpurpose</span><span class="sxs-lookup"><span data-stu-id="48377-138">userPurpose</span></span>|[<span data-ttu-id="48377-139">userpurpose</span><span class="sxs-lookup"><span data-stu-id="48377-139">userPurpose</span></span>](userpurpose.md)|<span data-ttu-id="48377-140">O objetivo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="48377-140">The purpose of the mailbox.</span></span> <span data-ttu-id="48377-141">Usado para diferenciar uma caixa de correio de um único usuário de uma caixa de correio compartilhada e caixa de correio de equipamento no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="48377-141">Used to differentiate a mailbox for a single user from a shared mailbox and equipment mailbox in Exchange Online.</span></span> <span data-ttu-id="48377-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="48377-142">Read only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48377-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48377-143">JSON representation</span></span>

<span data-ttu-id="48377-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48377-144">Here is a JSON representation of the resource.</span></span>

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
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"},
  "userPurpose": {"@odata.type": "microsoft.graph.userPurpose"}
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
