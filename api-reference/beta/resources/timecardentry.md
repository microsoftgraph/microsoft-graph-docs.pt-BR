---
title: Tipo de recurso timeCardEntry
description: Representa uma entrada de cartão de ponto específica.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d09b324b4d43765f05de789129021e2eb1f24789
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786369"
---
# <a name="timecardentry-resource-type"></a><span data-ttu-id="7710b-103">Tipo de recurso timeCardEntry</span><span class="sxs-lookup"><span data-stu-id="7710b-103">timeCardEntry resource type</span></span>

<span data-ttu-id="7710b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7710b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7710b-105">Representa uma entrada de cartão de ponto [específica.](timecard.md)</span><span class="sxs-lookup"><span data-stu-id="7710b-105">Represents a specific [timeCard](timecard.md) entry.</span></span>

## <a name="properties"></a><span data-ttu-id="7710b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7710b-106">Properties</span></span>
|<span data-ttu-id="7710b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7710b-107">Property</span></span>               |<span data-ttu-id="7710b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7710b-108">Type</span></span>           |<span data-ttu-id="7710b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7710b-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="7710b-110">clockInEvent</span><span class="sxs-lookup"><span data-stu-id="7710b-110">clockInEvent</span></span>       |[<span data-ttu-id="7710b-111">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="7710b-111">timeCardEvent</span></span>](timecardevent.md)    | <span data-ttu-id="7710b-112">O evento de clock-in do **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="7710b-112">The clock-in event of the **timeCard**.</span></span>|
| <span data-ttu-id="7710b-113">clockOutEvent</span><span class="sxs-lookup"><span data-stu-id="7710b-113">clockOutEvent</span></span>                 |[<span data-ttu-id="7710b-114">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="7710b-114">timeCardEvent</span></span>](timecardevent.md)  |<span data-ttu-id="7710b-115">O evento de saída do **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="7710b-115">The clock-out event of the **timeCard**.</span></span> |
| <span data-ttu-id="7710b-116">quebras</span><span class="sxs-lookup"><span data-stu-id="7710b-116">breaks</span></span>    |<span data-ttu-id="7710b-117">[Coleção timeCardBreak](timecardbreak.md)</span><span class="sxs-lookup"><span data-stu-id="7710b-117">[timeCardBreak](timecardbreak.md) collection</span></span>    |<span data-ttu-id="7710b-118">A lista de quebras associada ao **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="7710b-118">The list of breaks associated with the **timeCard**.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7710b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7710b-119">JSON representation</span></span>

<span data-ttu-id="7710b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7710b-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEntry"
}-->
```json
{
   "clockInEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "clockOutEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "string",
             "contentType": "text"
          },
         "start":{
            "dateTime":"String (timestamp)",
            "atApprovedLocation":true,
            "notes":{
                 "content": "string",
                 "contentType": "text"
            },
         },
         "end":null
      }
   ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timecardentry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
