---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a9fb455d2a67835ff1a3a10f89ee188a21e9956b
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822778"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="3d934-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="3d934-103">mailboxSettings resource type</span></span>

<span data-ttu-id="3d934-104">Configurações da caixa de correio principal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="3d934-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="3d934-105">Você pode [obter](../api/user-get-mailboxsettings.md) ou [Atualizar](../api/user-update-mailboxsettings.md) as configurações de caixa de correio de um usuário consultando a propriedade **mailboxSettings** do usuário.</span><span class="sxs-lookup"><span data-stu-id="3d934-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="3d934-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d934-106">Properties</span></span>
| <span data-ttu-id="3d934-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d934-107">Property</span></span>     | <span data-ttu-id="3d934-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d934-108">Type</span></span>   |<span data-ttu-id="3d934-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d934-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d934-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="3d934-110">archiveFolder</span></span>|<span data-ttu-id="3d934-111">string</span><span class="sxs-lookup"><span data-stu-id="3d934-111">string</span></span>|<span data-ttu-id="3d934-112">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="3d934-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="3d934-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="3d934-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="3d934-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="3d934-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="3d934-115">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="3d934-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="3d934-116">idioma</span><span class="sxs-lookup"><span data-stu-id="3d934-116">language</span></span>|[<span data-ttu-id="3d934-117">localeInfo</span><span class="sxs-lookup"><span data-stu-id="3d934-117">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="3d934-118">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="3d934-118">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="3d934-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="3d934-119">timeZone</span></span>|<span data-ttu-id="3d934-120">string</span><span class="sxs-lookup"><span data-stu-id="3d934-120">string</span></span>|<span data-ttu-id="3d934-121">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="3d934-121">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="3d934-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="3d934-122">workingHours</span></span>|[<span data-ttu-id="3d934-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="3d934-123">workingHours</span></span>](workinghours.md)|<span data-ttu-id="3d934-124">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="3d934-124">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d934-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d934-125">JSON representation</span></span>

<span data-ttu-id="3d934-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d934-126">Here is a JSON representation of the resource.</span></span>

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
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
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
