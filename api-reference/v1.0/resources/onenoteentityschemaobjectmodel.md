---
title: recurso de onenoteEntitySchemaObjectModel
description: Este é um tipo de base para entidades do OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 9ecdb17d48f8c8682af5970ea468fb2ad0118bbb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843880"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="5222e-103">recurso de onenoteEntitySchemaObjectModel</span><span class="sxs-lookup"><span data-stu-id="5222e-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="5222e-104">Este é um tipo de base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5222e-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5222e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5222e-105">JSON representation</span></span>

<span data-ttu-id="5222e-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5222e-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5222e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5222e-107">Properties</span></span>
| <span data-ttu-id="5222e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5222e-108">Property</span></span>     | <span data-ttu-id="5222e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5222e-109">Type</span></span>   |<span data-ttu-id="5222e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5222e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5222e-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5222e-111">createdDateTime</span></span>|<span data-ttu-id="5222e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5222e-112">DateTimeOffset</span></span>|<span data-ttu-id="5222e-p101">A data e a hora da criação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5222e-p101">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
