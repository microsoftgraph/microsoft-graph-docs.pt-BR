---
title: tipo de recurso de automaticRepliesMailTips
description: Dicas de email sobre qualquer respostas automáticas que foram configuradas em uma caixa de correio.
localization_priority: Normal
ms.openlocfilehash: 80ecaaa9fced0bcb00494b0414a86f0a11fd8996
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833226"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="9128f-103">tipo de recurso de automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="9128f-103">automaticRepliesMailTips resource type</span></span>

> <span data-ttu-id="9128f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9128f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9128f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9128f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9128f-106">[Dicas de email](../resources/mailtips.md) sobre qualquer respostas automáticas que foram configurados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9128f-106">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="9128f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9128f-107">Properties</span></span>
| <span data-ttu-id="9128f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9128f-108">Property</span></span>     | <span data-ttu-id="9128f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9128f-109">Type</span></span>   |<span data-ttu-id="9128f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9128f-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="9128f-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="9128f-111">message</span></span> | <span data-ttu-id="9128f-112">String</span><span class="sxs-lookup"><span data-stu-id="9128f-112">String</span></span> | <span data-ttu-id="9128f-113">A mensagem de resposta automática.</span><span class="sxs-lookup"><span data-stu-id="9128f-113">The automatic reply message.</span></span> |
| <span data-ttu-id="9128f-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="9128f-114">messageLanguage</span></span> | [<span data-ttu-id="9128f-115">localeInfo</span><span class="sxs-lookup"><span data-stu-id="9128f-115">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="9128f-116">O idioma em que a mensagem de resposta automática está em.</span><span class="sxs-lookup"><span data-stu-id="9128f-116">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="9128f-117">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="9128f-117">scheduledEndTime</span></span> | [<span data-ttu-id="9128f-118">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9128f-118">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="9128f-119">A data e hora em que as respostas automáticas estão definidas para encerrar.</span><span class="sxs-lookup"><span data-stu-id="9128f-119">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="9128f-120">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="9128f-120">scheduledStartTime</span></span> | [<span data-ttu-id="9128f-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9128f-121">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="9128f-122">A data e hora em que as respostas automáticas estão definidas para começar.</span><span class="sxs-lookup"><span data-stu-id="9128f-122">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9128f-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9128f-123">JSON representation</span></span>

<span data-ttu-id="9128f-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9128f-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
