---
title: Tipo de recurso attendee
description: Um participante do evento. Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cadb1ca6d2ab1168c3c7f9ff2b182b57112bfb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532088"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="ffc3b-104">Tipo de recurso attendee</span><span class="sxs-lookup"><span data-stu-id="ffc3b-104">attendee resource type</span></span>

<span data-ttu-id="ffc3b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffc3b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffc3b-106">Um participante do evento.</span><span class="sxs-lookup"><span data-stu-id="ffc3b-106">An event attendee.</span></span> <span data-ttu-id="ffc3b-107">Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ffc3b-107">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="ffc3b-108">Derivado de [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="ffc3b-108">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ffc3b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ffc3b-109">Properties</span></span>
| <span data-ttu-id="ffc3b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffc3b-110">Property</span></span>     | <span data-ttu-id="ffc3b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffc3b-111">Type</span></span>   |<span data-ttu-id="ffc3b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffc3b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffc3b-113">status</span><span class="sxs-lookup"><span data-stu-id="ffc3b-113">status</span></span>|[<span data-ttu-id="ffc3b-114">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="ffc3b-114">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="ffc3b-115">A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.</span><span class="sxs-lookup"><span data-stu-id="ffc3b-115">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="ffc3b-116">type</span><span class="sxs-lookup"><span data-stu-id="ffc3b-116">type</span></span>|<span data-ttu-id="ffc3b-117">String</span><span class="sxs-lookup"><span data-stu-id="ffc3b-117">String</span></span>|<span data-ttu-id="ffc3b-118">O tipo de participante: `required`, `optional` ou `resource`.</span><span class="sxs-lookup"><span data-stu-id="ffc3b-118">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="ffc3b-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ffc3b-119">emailAddress</span></span>|[<span data-ttu-id="ffc3b-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ffc3b-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ffc3b-121">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="ffc3b-121">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffc3b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffc3b-122">JSON representation</span></span>

<span data-ttu-id="ffc3b-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ffc3b-123">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
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
