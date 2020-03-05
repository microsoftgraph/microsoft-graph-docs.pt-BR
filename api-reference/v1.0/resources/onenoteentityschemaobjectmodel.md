---
title: recurso onenoteEntitySchemaObjectModel
description: Este é um tipo base para entidades do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 7f0d0d23d56091db051352eaa8bde7668829e5da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447315"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="92d08-103">recurso onenoteEntitySchemaObjectModel</span><span class="sxs-lookup"><span data-stu-id="92d08-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="92d08-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92d08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92d08-105">Este é um tipo base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="92d08-105">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="92d08-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92d08-106">JSON representation</span></span>

<span data-ttu-id="92d08-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92d08-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="92d08-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92d08-108">Properties</span></span>
| <span data-ttu-id="92d08-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92d08-109">Property</span></span>     | <span data-ttu-id="92d08-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="92d08-110">Type</span></span>   |<span data-ttu-id="92d08-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="92d08-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92d08-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92d08-112">createdDateTime</span></span>|<span data-ttu-id="92d08-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92d08-113">DateTimeOffset</span></span>|<span data-ttu-id="92d08-114">A data e a hora em que a página foi criada.</span><span class="sxs-lookup"><span data-stu-id="92d08-114">The date and time when the page was created.</span></span> <span data-ttu-id="92d08-115">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="92d08-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92d08-116">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="92d08-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="92d08-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92d08-117">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
