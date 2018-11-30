---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
ms.openlocfilehash: 2d7d3889cd65886eba4cf9356862417928ed3296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033140"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="2c9c2-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="2c9c2-103">attendeeBase resource type</span></span>

> <span data-ttu-id="2c9c2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2c9c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c9c2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2c9c2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c9c2-106">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="2c9c2-106">The type of attendee.</span></span>

<span data-ttu-id="2c9c2-107">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="2c9c2-107">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c9c2-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c9c2-108">JSON representation</span></span>

<span data-ttu-id="2c9c2-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2c9c2-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="2c9c2-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c9c2-110">Properties</span></span>
| <span data-ttu-id="2c9c2-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c9c2-111">Property</span></span>     | <span data-ttu-id="2c9c2-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c9c2-112">Type</span></span>   |<span data-ttu-id="2c9c2-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c9c2-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c9c2-114">type</span><span class="sxs-lookup"><span data-stu-id="2c9c2-114">type</span></span>|<span data-ttu-id="2c9c2-115">String</span><span class="sxs-lookup"><span data-stu-id="2c9c2-115">String</span></span>| <span data-ttu-id="2c9c2-p102">O tipo de participante. Os valores possíveis são: `required`, `optional`, `resource`. Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="2c9c2-p102">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="2c9c2-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2c9c2-119">emailAddress</span></span>|[<span data-ttu-id="2c9c2-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2c9c2-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="2c9c2-121">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="2c9c2-121">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->