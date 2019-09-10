---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 63340e1edd86ad61c48d707ef0bff685a57c3ef8
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822729"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="5b484-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="5b484-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b484-104">Configurações da caixa de correio principal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="5b484-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="5b484-105">Você pode [obter](../api/user-get-mailboxsettings.md) ou [Atualizar](../api/user-update-mailboxsettings.md) as configurações de caixa de correio de um usuário consultando a propriedade **mailboxSettings** do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b484-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="5b484-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b484-106">Properties</span></span>
| <span data-ttu-id="5b484-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b484-107">Property</span></span>     | <span data-ttu-id="5b484-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b484-108">Type</span></span>   |<span data-ttu-id="5b484-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b484-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b484-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="5b484-110">archiveFolder</span></span>|<span data-ttu-id="5b484-111">string</span><span class="sxs-lookup"><span data-stu-id="5b484-111">string</span></span>|<span data-ttu-id="5b484-112">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b484-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="5b484-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="5b484-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="5b484-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="5b484-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="5b484-115">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5b484-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="5b484-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="5b484-116">dateFormat</span></span>|<span data-ttu-id="5b484-117">string</span><span class="sxs-lookup"><span data-stu-id="5b484-117">string</span></span>|<span data-ttu-id="5b484-118">O formato de data da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b484-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="5b484-119">idioma</span><span class="sxs-lookup"><span data-stu-id="5b484-119">language</span></span>|[<span data-ttu-id="5b484-120">localeInfo</span><span class="sxs-lookup"><span data-stu-id="5b484-120">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="5b484-121">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="5b484-121">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="5b484-122">Formato de TimeFormat</span><span class="sxs-lookup"><span data-stu-id="5b484-122">timeFormat</span></span>|<span data-ttu-id="5b484-123">string</span><span class="sxs-lookup"><span data-stu-id="5b484-123">string</span></span>|<span data-ttu-id="5b484-124">O formato de hora da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b484-124">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="5b484-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="5b484-125">timeZone</span></span>|<span data-ttu-id="5b484-126">string</span><span class="sxs-lookup"><span data-stu-id="5b484-126">string</span></span>|<span data-ttu-id="5b484-127">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b484-127">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="5b484-128">workingHours</span><span class="sxs-lookup"><span data-stu-id="5b484-128">workingHours</span></span>|[<span data-ttu-id="5b484-129">workingHours</span><span class="sxs-lookup"><span data-stu-id="5b484-129">workingHours</span></span>](workinghours.md)|<span data-ttu-id="5b484-130">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="5b484-130">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b484-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b484-131">JSON representation</span></span>

<span data-ttu-id="5b484-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b484-132">Here is a JSON representation of the resource.</span></span>

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
