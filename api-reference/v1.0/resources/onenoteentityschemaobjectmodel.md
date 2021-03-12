---
title: Recurso onenoteEntitySchemaObjectModel
description: Esse é um tipo base para entidades do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 9dd44c3360a58195f04632b849f5cafd73490676
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722332"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="36aea-103">Recurso onenoteEntitySchemaObjectModel</span><span class="sxs-lookup"><span data-stu-id="36aea-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="36aea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36aea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36aea-105">Esse é um tipo base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="36aea-105">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36aea-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36aea-106">JSON representation</span></span>

<span data-ttu-id="36aea-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36aea-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntitySchemaObjectModel"
}-->

```json
{
  "createdDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="36aea-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36aea-108">Properties</span></span>
| <span data-ttu-id="36aea-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36aea-109">Property</span></span>     | <span data-ttu-id="36aea-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="36aea-110">Type</span></span>   |<span data-ttu-id="36aea-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="36aea-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36aea-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36aea-112">createdDateTime</span></span>|<span data-ttu-id="36aea-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36aea-113">DateTimeOffset</span></span>|<span data-ttu-id="36aea-114">A data e a hora em que a página foi criada.</span><span class="sxs-lookup"><span data-stu-id="36aea-114">The date and time when the page was created.</span></span> <span data-ttu-id="36aea-115">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="36aea-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="36aea-116">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="36aea-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="36aea-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36aea-117">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

