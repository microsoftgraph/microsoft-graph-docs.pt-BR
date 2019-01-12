---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6ad2a215270e712e8438e9d2b4b8ce2803477192
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980122"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="20d99-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="20d99-103">mailboxSettings resource type</span></span>

> <span data-ttu-id="20d99-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="20d99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20d99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="20d99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20d99-106">Configurações para a caixa de correio principal do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="20d99-106">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="20d99-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20d99-107">Properties</span></span>
| <span data-ttu-id="20d99-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20d99-108">Property</span></span>     | <span data-ttu-id="20d99-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="20d99-109">Type</span></span>   |<span data-ttu-id="20d99-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="20d99-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20d99-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="20d99-111">archiveFolder</span></span>|<span data-ttu-id="20d99-112">string</span><span class="sxs-lookup"><span data-stu-id="20d99-112">string</span></span>|<span data-ttu-id="20d99-113">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="20d99-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="20d99-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="20d99-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="20d99-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="20d99-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="20d99-116">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="20d99-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="20d99-117">idioma</span><span class="sxs-lookup"><span data-stu-id="20d99-117">language</span></span>|[<span data-ttu-id="20d99-118">localeInfo</span><span class="sxs-lookup"><span data-stu-id="20d99-118">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="20d99-119">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="20d99-119">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="20d99-120">timeZone</span><span class="sxs-lookup"><span data-stu-id="20d99-120">timeZone</span></span>|<span data-ttu-id="20d99-121">string</span><span class="sxs-lookup"><span data-stu-id="20d99-121">string</span></span>|<span data-ttu-id="20d99-122">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="20d99-122">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="20d99-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="20d99-123">workingHours</span></span>|[<span data-ttu-id="20d99-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="20d99-124">workingHours</span></span>](workinghours.md)|<span data-ttu-id="20d99-125">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="20d99-125">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20d99-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20d99-126">JSON representation</span></span>

<span data-ttu-id="20d99-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20d99-127">Here is a JSON representation of the resource.</span></span>

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
