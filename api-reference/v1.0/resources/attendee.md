---
title: Tipo de recurso attendee
description: Um participante do evento. Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0d679704cf884276718186c289ded0c8d5bb05df
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033100"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="b53ad-104">Tipo de recurso attendee</span><span class="sxs-lookup"><span data-stu-id="b53ad-104">attendee resource type</span></span>

<span data-ttu-id="b53ad-105">Um participante do evento.</span><span class="sxs-lookup"><span data-stu-id="b53ad-105">An event attendee.</span></span> <span data-ttu-id="b53ad-106">Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b53ad-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="b53ad-107">Derivado de [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="b53ad-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b53ad-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b53ad-108">Properties</span></span>
| <span data-ttu-id="b53ad-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b53ad-109">Property</span></span>     | <span data-ttu-id="b53ad-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b53ad-110">Type</span></span>   |<span data-ttu-id="b53ad-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b53ad-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b53ad-112">status</span><span class="sxs-lookup"><span data-stu-id="b53ad-112">status</span></span>|[<span data-ttu-id="b53ad-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="b53ad-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="b53ad-114">A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.</span><span class="sxs-lookup"><span data-stu-id="b53ad-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="b53ad-115">type</span><span class="sxs-lookup"><span data-stu-id="b53ad-115">type</span></span>|<span data-ttu-id="b53ad-116">String</span><span class="sxs-lookup"><span data-stu-id="b53ad-116">String</span></span>|<span data-ttu-id="b53ad-117">O tipo de participante: `required`, `optional` ou `resource`.</span><span class="sxs-lookup"><span data-stu-id="b53ad-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="b53ad-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b53ad-118">emailAddress</span></span>|[<span data-ttu-id="b53ad-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b53ad-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="b53ad-120">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="b53ad-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b53ad-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b53ad-121">JSON representation</span></span>

<span data-ttu-id="b53ad-122">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b53ad-122">Here is a JSON representation of the resource</span></span>

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
