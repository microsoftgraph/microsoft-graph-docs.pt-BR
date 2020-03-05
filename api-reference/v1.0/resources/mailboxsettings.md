---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 99097c026ef219e82a34a6c7b043cf70d36c965d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447504"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="a658f-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="a658f-103">mailboxSettings resource type</span></span>

<span data-ttu-id="a658f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a658f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a658f-105">Configurações da caixa de correio principal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="a658f-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="a658f-106">Você pode [obter](../api/user-get-mailboxsettings.md) ou [Atualizar](../api/user-update-mailboxsettings.md) as configurações de caixa de correio de um usuário consultando a propriedade **mailboxSettings** do usuário.</span><span class="sxs-lookup"><span data-stu-id="a658f-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="a658f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a658f-107">Properties</span></span>
| <span data-ttu-id="a658f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a658f-108">Property</span></span>     | <span data-ttu-id="a658f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a658f-109">Type</span></span>   |<span data-ttu-id="a658f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a658f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a658f-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="a658f-111">archiveFolder</span></span>|<span data-ttu-id="a658f-112">string</span><span class="sxs-lookup"><span data-stu-id="a658f-112">string</span></span>|<span data-ttu-id="a658f-113">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="a658f-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="a658f-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="a658f-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="a658f-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="a658f-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="a658f-116">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a658f-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="a658f-117">dateFormat</span><span class="sxs-lookup"><span data-stu-id="a658f-117">dateFormat</span></span>|<span data-ttu-id="a658f-118">string</span><span class="sxs-lookup"><span data-stu-id="a658f-118">string</span></span>|<span data-ttu-id="a658f-119">O formato de data da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a658f-119">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="a658f-120">idioma</span><span class="sxs-lookup"><span data-stu-id="a658f-120">language</span></span>|[<span data-ttu-id="a658f-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="a658f-121">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="a658f-122">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="a658f-122">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="a658f-123">Formato de TimeFormat</span><span class="sxs-lookup"><span data-stu-id="a658f-123">timeFormat</span></span>|<span data-ttu-id="a658f-124">string</span><span class="sxs-lookup"><span data-stu-id="a658f-124">string</span></span>|<span data-ttu-id="a658f-125">O formato de hora da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a658f-125">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="a658f-126">timeZone</span><span class="sxs-lookup"><span data-stu-id="a658f-126">timeZone</span></span>|<span data-ttu-id="a658f-127">string</span><span class="sxs-lookup"><span data-stu-id="a658f-127">string</span></span>|<span data-ttu-id="a658f-128">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a658f-128">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="a658f-129">workingHours</span><span class="sxs-lookup"><span data-stu-id="a658f-129">workingHours</span></span>|[<span data-ttu-id="a658f-130">workingHours</span><span class="sxs-lookup"><span data-stu-id="a658f-130">workingHours</span></span>](workinghours.md)|<span data-ttu-id="a658f-131">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="a658f-131">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a658f-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a658f-132">JSON representation</span></span>

<span data-ttu-id="a658f-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a658f-133">Here is a JSON representation of the resource.</span></span>

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
