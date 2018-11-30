---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
ms.openlocfilehash: 79a01c59ec0a891c13107095a950a7cc8ae0b547
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033207"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="eaa26-103">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="eaa26-103">mailboxSettings resource type</span></span>

> <span data-ttu-id="eaa26-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eaa26-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaa26-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eaa26-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eaa26-106">Configurações para a caixa de correio principal do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="eaa26-106">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="eaa26-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eaa26-107">Properties</span></span>
| <span data-ttu-id="eaa26-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaa26-108">Property</span></span>     | <span data-ttu-id="eaa26-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaa26-109">Type</span></span>   |<span data-ttu-id="eaa26-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa26-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eaa26-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="eaa26-111">archiveFolder</span></span>|<span data-ttu-id="eaa26-112">string</span><span class="sxs-lookup"><span data-stu-id="eaa26-112">string</span></span>|<span data-ttu-id="eaa26-113">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="eaa26-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="eaa26-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="eaa26-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="eaa26-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="eaa26-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="eaa26-116">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="eaa26-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="eaa26-117">idioma</span><span class="sxs-lookup"><span data-stu-id="eaa26-117">language</span></span>|[<span data-ttu-id="eaa26-118">localeInfo</span><span class="sxs-lookup"><span data-stu-id="eaa26-118">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="eaa26-119">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="eaa26-119">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="eaa26-120">timeZone</span><span class="sxs-lookup"><span data-stu-id="eaa26-120">timeZone</span></span>|<span data-ttu-id="eaa26-121">string</span><span class="sxs-lookup"><span data-stu-id="eaa26-121">string</span></span>|<span data-ttu-id="eaa26-122">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="eaa26-122">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="eaa26-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="eaa26-123">workingHours</span></span>|[<span data-ttu-id="eaa26-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="eaa26-124">workingHours</span></span>](workinghours.md)|<span data-ttu-id="eaa26-125">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="eaa26-125">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eaa26-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eaa26-126">JSON representation</span></span>

<span data-ttu-id="eaa26-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eaa26-127">Here is a JSON representation of the resource.</span></span>

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