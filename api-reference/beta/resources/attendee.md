---
title: Tipo de recurso attendee
description: Um participante do evento. Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.
ms.openlocfilehash: 7c1a4d5fb483dc722768c9b95885837bdaf6087e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037870"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="1c320-104">Tipo de recurso attendee</span><span class="sxs-lookup"><span data-stu-id="1c320-104">attendee resource type</span></span>

> <span data-ttu-id="1c320-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1c320-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c320-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1c320-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c320-107">Um participante do evento.</span><span class="sxs-lookup"><span data-stu-id="1c320-107">An event attendee.</span></span> <span data-ttu-id="1c320-108">Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c320-108">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="1c320-109">Derivado de [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="1c320-109">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1c320-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c320-110">Properties</span></span>
| <span data-ttu-id="1c320-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c320-111">Property</span></span>     | <span data-ttu-id="1c320-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c320-112">Type</span></span>   |<span data-ttu-id="1c320-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c320-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c320-114">status</span><span class="sxs-lookup"><span data-stu-id="1c320-114">status</span></span>|[<span data-ttu-id="1c320-115">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="1c320-115">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="1c320-116">A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.</span><span class="sxs-lookup"><span data-stu-id="1c320-116">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="1c320-117">type</span><span class="sxs-lookup"><span data-stu-id="1c320-117">type</span></span>|<span data-ttu-id="1c320-118">String</span><span class="sxs-lookup"><span data-stu-id="1c320-118">String</span></span>|<span data-ttu-id="1c320-119">O tipo de participante: `required`, `optional` ou `resource`.</span><span class="sxs-lookup"><span data-stu-id="1c320-119">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="1c320-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1c320-120">emailAddress</span></span>|[<span data-ttu-id="1c320-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1c320-121">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="1c320-122">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="1c320-122">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c320-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c320-123">JSON representation</span></span>

<span data-ttu-id="1c320-124">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1c320-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->