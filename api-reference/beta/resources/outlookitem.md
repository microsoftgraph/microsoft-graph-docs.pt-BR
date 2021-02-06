---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 10a4bd64fd8776b1d50d52d5fd9130076417dc85
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128593"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="6f899-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="6f899-103">outlookItem resource type</span></span>

<span data-ttu-id="6f899-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f899-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="6f899-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f899-105">JSON representation</span></span>

<span data-ttu-id="6f899-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6f899-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6f899-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f899-107">Properties</span></span>
| <span data-ttu-id="6f899-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f899-108">Property</span></span>     | <span data-ttu-id="6f899-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f899-109">Type</span></span>   |<span data-ttu-id="6f899-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f899-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f899-111">categories</span><span class="sxs-lookup"><span data-stu-id="6f899-111">categories</span></span>|<span data-ttu-id="6f899-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f899-112">String collection</span></span>||
|<span data-ttu-id="6f899-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="6f899-113">changeKey</span></span>|<span data-ttu-id="6f899-114">String</span><span class="sxs-lookup"><span data-stu-id="6f899-114">String</span></span>||
|<span data-ttu-id="6f899-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f899-115">createdDateTime</span></span>|<span data-ttu-id="6f899-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f899-116">DateTimeOffset</span></span>|<span data-ttu-id="6f899-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6f899-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6f899-119">id</span><span class="sxs-lookup"><span data-stu-id="6f899-119">id</span></span>|<span data-ttu-id="6f899-120">String</span><span class="sxs-lookup"><span data-stu-id="6f899-120">String</span></span>| <span data-ttu-id="6f899-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f899-121">Read-only.</span></span>|
|<span data-ttu-id="6f899-122">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f899-122">lastModifiedDateTime</span></span>|<span data-ttu-id="6f899-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f899-123">DateTimeOffset</span></span>|<span data-ttu-id="6f899-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6f899-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f899-126">Relações</span><span class="sxs-lookup"><span data-stu-id="6f899-126">Relationships</span></span>
<span data-ttu-id="6f899-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6f899-127">None</span></span>


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


