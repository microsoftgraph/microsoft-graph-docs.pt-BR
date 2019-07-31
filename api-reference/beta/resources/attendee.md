---
title: Tipo de recurso attendee
description: Um participante do evento. Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 435a9b3badf20ddb79affd4e40e5ca8b66ff34c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974287"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="bf352-104">Tipo de recurso attendee</span><span class="sxs-lookup"><span data-stu-id="bf352-104">attendee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf352-105">Um participante do evento.</span><span class="sxs-lookup"><span data-stu-id="bf352-105">An event attendee.</span></span> <span data-ttu-id="bf352-106">Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf352-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="bf352-107">Derivado de [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="bf352-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bf352-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf352-108">Properties</span></span>
| <span data-ttu-id="bf352-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf352-109">Property</span></span>     | <span data-ttu-id="bf352-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf352-110">Type</span></span>   |<span data-ttu-id="bf352-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf352-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf352-112">status</span><span class="sxs-lookup"><span data-stu-id="bf352-112">status</span></span>|[<span data-ttu-id="bf352-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="bf352-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="bf352-114">A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.</span><span class="sxs-lookup"><span data-stu-id="bf352-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="bf352-115">type</span><span class="sxs-lookup"><span data-stu-id="bf352-115">type</span></span>|<span data-ttu-id="bf352-116">String</span><span class="sxs-lookup"><span data-stu-id="bf352-116">String</span></span>|<span data-ttu-id="bf352-117">O tipo de participante: `required`, `optional` ou `resource`.</span><span class="sxs-lookup"><span data-stu-id="bf352-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="bf352-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bf352-118">emailAddress</span></span>|[<span data-ttu-id="bf352-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bf352-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="bf352-120">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="bf352-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf352-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf352-121">JSON representation</span></span>

<span data-ttu-id="bf352-122">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bf352-122">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
