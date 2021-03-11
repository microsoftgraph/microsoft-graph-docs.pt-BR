---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9ed43ccabfbd2b5389525ebec02ecd04edb475b3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721814"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="c98be-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="c98be-103">outlookItem resource type</span></span>

<span data-ttu-id="c98be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c98be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="c98be-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c98be-105">JSON representation</span></span>

<span data-ttu-id="c98be-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c98be-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookItem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="c98be-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c98be-107">Properties</span></span>
| <span data-ttu-id="c98be-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c98be-108">Property</span></span>     | <span data-ttu-id="c98be-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c98be-109">Type</span></span>   |<span data-ttu-id="c98be-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c98be-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c98be-111">categories</span><span class="sxs-lookup"><span data-stu-id="c98be-111">categories</span></span>|<span data-ttu-id="c98be-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c98be-112">String collection</span></span>||
|<span data-ttu-id="c98be-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="c98be-113">changeKey</span></span>|<span data-ttu-id="c98be-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c98be-114">String</span></span>||
|<span data-ttu-id="c98be-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c98be-115">createdDateTime</span></span>|<span data-ttu-id="c98be-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c98be-116">DateTimeOffset</span></span>|<span data-ttu-id="c98be-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c98be-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c98be-118">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="c98be-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="c98be-119">id</span><span class="sxs-lookup"><span data-stu-id="c98be-119">id</span></span>|<span data-ttu-id="c98be-120">String</span><span class="sxs-lookup"><span data-stu-id="c98be-120">String</span></span>| <span data-ttu-id="c98be-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c98be-121">Read-only.</span></span>|
|<span data-ttu-id="c98be-122">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c98be-122">lastModifiedDateTime</span></span>|<span data-ttu-id="c98be-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c98be-123">DateTimeOffset</span></span>|<span data-ttu-id="c98be-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c98be-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c98be-125">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="c98be-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="c98be-126">Relações</span><span class="sxs-lookup"><span data-stu-id="c98be-126">Relationships</span></span>
<span data-ttu-id="c98be-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c98be-127">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


