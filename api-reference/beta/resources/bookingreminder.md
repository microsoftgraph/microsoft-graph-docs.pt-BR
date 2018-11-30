---
title: tipo de recurso de bookingReminder
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: f5f7b30c296433dd96ffa14a75e3f0286e8a16a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037338"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="a2044-104">tipo de recurso de bookingReminder</span><span class="sxs-lookup"><span data-stu-id="a2044-104">bookingReminder resource type</span></span>

 > <span data-ttu-id="a2044-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a2044-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2044-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a2044-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="a2044-107">Representa quando e para os quais enviar um lembrete de email.</span><span class="sxs-lookup"><span data-stu-id="a2044-107">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="a2044-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2044-108">Properties</span></span>
| <span data-ttu-id="a2044-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2044-109">Property</span></span>     | <span data-ttu-id="a2044-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2044-110">Type</span></span>   |<span data-ttu-id="a2044-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2044-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2044-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="a2044-112">message</span></span>|<span data-ttu-id="a2044-113">String</span><span class="sxs-lookup"><span data-stu-id="a2044-113">String</span></span>|<span data-ttu-id="a2044-114">A mensagem do lembrete.</span><span class="sxs-lookup"><span data-stu-id="a2044-114">The message in the reminder.</span></span>|
|<span data-ttu-id="a2044-115">deslocamento</span><span class="sxs-lookup"><span data-stu-id="a2044-115">offset</span></span>|<span data-ttu-id="a2044-116">Duração</span><span class="sxs-lookup"><span data-stu-id="a2044-116">Duration</span></span>|<span data-ttu-id="a2044-117">A quantidade de tempo antes do início de um compromisso que o lembrete deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="a2044-117">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="a2044-118">Ele é indicado no formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="a2044-118">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="a2044-119">recipients</span><span class="sxs-lookup"><span data-stu-id="a2044-119">recipients</span></span>|<span data-ttu-id="a2044-120">String</span><span class="sxs-lookup"><span data-stu-id="a2044-120">String</span></span>| <span data-ttu-id="a2044-121">As pessoas que recebem shouold o lembrete.</span><span class="sxs-lookup"><span data-stu-id="a2044-121">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="a2044-122">Os valores possíveis são: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="a2044-122">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2044-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2044-123">JSON representation</span></span>

<span data-ttu-id="a2044-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2044-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->