---
title: recurso onenoteEntitySchemaObjectModel
description: Este é um tipo base para entidades do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 4072a6d02ffb003731613c081effac50215f605a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035809"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="ff0b4-103">recurso onenoteEntitySchemaObjectModel</span><span class="sxs-lookup"><span data-stu-id="ff0b4-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="ff0b4-104">Este é um tipo base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="ff0b4-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff0b4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff0b4-105">JSON representation</span></span>

<span data-ttu-id="ff0b4-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff0b4-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ff0b4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff0b4-107">Properties</span></span>
| <span data-ttu-id="ff0b4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff0b4-108">Property</span></span>     | <span data-ttu-id="ff0b4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff0b4-109">Type</span></span>   |<span data-ttu-id="ff0b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff0b4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff0b4-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff0b4-111">createdDateTime</span></span>|<span data-ttu-id="ff0b4-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff0b4-112">DateTimeOffset</span></span>|<span data-ttu-id="ff0b4-113">A data e a hora em que a página foi criada.</span><span class="sxs-lookup"><span data-stu-id="ff0b4-113">The date and time when the page was created.</span></span> <span data-ttu-id="ff0b4-114">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ff0b4-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ff0b4-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ff0b4-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ff0b4-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff0b4-116">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
