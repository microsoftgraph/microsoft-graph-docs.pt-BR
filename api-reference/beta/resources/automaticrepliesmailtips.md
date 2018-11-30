---
title: tipo de recurso de automaticRepliesMailTips
description: Dicas de email sobre qualquer respostas automáticas que foram configuradas em uma caixa de correio.
ms.openlocfilehash: 51657578474710d40cfc3feabdf41e50e7105942
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040888"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="c5f52-103">tipo de recurso de automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="c5f52-103">automaticRepliesMailTips resource type</span></span>

> <span data-ttu-id="c5f52-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c5f52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5f52-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c5f52-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5f52-106">[Dicas de email](../resources/mailtips.md) sobre qualquer respostas automáticas que foram configurados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c5f52-106">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="c5f52-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5f52-107">Properties</span></span>
| <span data-ttu-id="c5f52-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5f52-108">Property</span></span>     | <span data-ttu-id="c5f52-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5f52-109">Type</span></span>   |<span data-ttu-id="c5f52-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f52-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="c5f52-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="c5f52-111">message</span></span> | <span data-ttu-id="c5f52-112">String</span><span class="sxs-lookup"><span data-stu-id="c5f52-112">String</span></span> | <span data-ttu-id="c5f52-113">A mensagem de resposta automática.</span><span class="sxs-lookup"><span data-stu-id="c5f52-113">The automatic reply message.</span></span> |
| <span data-ttu-id="c5f52-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="c5f52-114">messageLanguage</span></span> | [<span data-ttu-id="c5f52-115">localeInfo</span><span class="sxs-lookup"><span data-stu-id="c5f52-115">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="c5f52-116">O idioma em que a mensagem de resposta automática está em.</span><span class="sxs-lookup"><span data-stu-id="c5f52-116">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="c5f52-117">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="c5f52-117">scheduledEndTime</span></span> | [<span data-ttu-id="c5f52-118">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c5f52-118">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="c5f52-119">A data e hora em que as respostas automáticas estão definidas para encerrar.</span><span class="sxs-lookup"><span data-stu-id="c5f52-119">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="c5f52-120">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="c5f52-120">scheduledStartTime</span></span> | [<span data-ttu-id="c5f52-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c5f52-121">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="c5f52-122">A data e hora em que as respostas automáticas estão definidas para começar.</span><span class="sxs-lookup"><span data-stu-id="c5f52-122">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5f52-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5f52-123">JSON representation</span></span>

<span data-ttu-id="c5f52-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5f52-124">Here is a JSON representation of the resource.</span></span>

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