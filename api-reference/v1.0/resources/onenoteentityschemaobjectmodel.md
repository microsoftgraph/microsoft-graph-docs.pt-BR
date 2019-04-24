---
title: recurso onenoteEntitySchemaObjectModel
description: Este é um tipo base para entidades do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 168359bbdaa659db461aa33af96e402a4a81783d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462589"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="e342e-103">recurso onenoteEntitySchemaObjectModel</span><span class="sxs-lookup"><span data-stu-id="e342e-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="e342e-104">Este é um tipo base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e342e-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e342e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e342e-105">JSON representation</span></span>

<span data-ttu-id="e342e-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e342e-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e342e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e342e-107">Properties</span></span>
| <span data-ttu-id="e342e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e342e-108">Property</span></span>     | <span data-ttu-id="e342e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e342e-109">Type</span></span>   |<span data-ttu-id="e342e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e342e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e342e-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e342e-111">createdDateTime</span></span>|<span data-ttu-id="e342e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e342e-112">DateTimeOffset</span></span>|<span data-ttu-id="e342e-113">A data e a hora em que a página foi criada.</span><span class="sxs-lookup"><span data-stu-id="e342e-113">The date and time when the page was created.</span></span> <span data-ttu-id="e342e-114">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e342e-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e342e-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e342e-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e342e-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e342e-116">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
