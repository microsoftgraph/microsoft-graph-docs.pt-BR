---
title: recurso de onenoteEntitySchemaObjectModel
description: Este é um tipo de base para entidades do OneNote.
author: Jewan-microsoft
ms.openlocfilehash: a44d05a512b8e4ed2615296faae3f35bd7bd554f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319443"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="98362-103">recurso de onenoteEntitySchemaObjectModel</span><span class="sxs-lookup"><span data-stu-id="98362-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="98362-104">Este é um tipo de base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="98362-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98362-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98362-105">JSON representation</span></span>

<span data-ttu-id="98362-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98362-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="98362-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98362-107">Properties</span></span>
| <span data-ttu-id="98362-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98362-108">Property</span></span>     | <span data-ttu-id="98362-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="98362-109">Type</span></span>   |<span data-ttu-id="98362-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="98362-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98362-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98362-111">createdDateTime</span></span>|<span data-ttu-id="98362-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98362-112">DateTimeOffset</span></span>|<span data-ttu-id="98362-p101">A data e a hora da criação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="98362-p101">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->