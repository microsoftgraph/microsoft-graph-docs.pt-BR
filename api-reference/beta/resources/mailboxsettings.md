---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bf5ca7b6e9a653946f5ea1ff0a302c8499f2e02d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345114"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="07be5-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="07be5-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07be5-104">Configurações para a caixa de correio principal do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="07be5-104">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="07be5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07be5-105">Properties</span></span>
| <span data-ttu-id="07be5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07be5-106">Property</span></span>     | <span data-ttu-id="07be5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="07be5-107">Type</span></span>   |<span data-ttu-id="07be5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="07be5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07be5-109">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="07be5-109">archiveFolder</span></span>|<span data-ttu-id="07be5-110">string</span><span class="sxs-lookup"><span data-stu-id="07be5-110">string</span></span>|<span data-ttu-id="07be5-111">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="07be5-111">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="07be5-112">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="07be5-112">automaticRepliesSetting</span></span>|[<span data-ttu-id="07be5-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="07be5-113">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="07be5-114">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="07be5-114">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="07be5-115">idioma</span><span class="sxs-lookup"><span data-stu-id="07be5-115">language</span></span>|[<span data-ttu-id="07be5-116">localeInfo</span><span class="sxs-lookup"><span data-stu-id="07be5-116">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="07be5-117">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="07be5-117">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="07be5-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="07be5-118">timeZone</span></span>|<span data-ttu-id="07be5-119">string</span><span class="sxs-lookup"><span data-stu-id="07be5-119">string</span></span>|<span data-ttu-id="07be5-120">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="07be5-120">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="07be5-121">workingHours</span><span class="sxs-lookup"><span data-stu-id="07be5-121">workingHours</span></span>|[<span data-ttu-id="07be5-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="07be5-122">workingHours</span></span>](workinghours.md)|<span data-ttu-id="07be5-123">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="07be5-123">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07be5-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07be5-124">JSON representation</span></span>

<span data-ttu-id="07be5-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07be5-125">Here is a JSON representation of the resource.</span></span>

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
