---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 77741fa05f356418e688cdc4a45c5a4750604c3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009276"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="a9f8d-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="a9f8d-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="a9f8d-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9f8d-104">JSON representation</span></span>

<span data-ttu-id="a9f8d-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a9f8d-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a9f8d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9f8d-106">Properties</span></span>
| <span data-ttu-id="a9f8d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9f8d-107">Property</span></span>     | <span data-ttu-id="a9f8d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9f8d-108">Type</span></span>   |<span data-ttu-id="a9f8d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9f8d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9f8d-110">categories</span><span class="sxs-lookup"><span data-stu-id="a9f8d-110">categories</span></span>|<span data-ttu-id="a9f8d-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9f8d-111">String collection</span></span>||
|<span data-ttu-id="a9f8d-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="a9f8d-112">changeKey</span></span>|<span data-ttu-id="a9f8d-113">String</span><span class="sxs-lookup"><span data-stu-id="a9f8d-113">String</span></span>||
|<span data-ttu-id="a9f8d-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f8d-114">createdDateTime</span></span>|<span data-ttu-id="a9f8d-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f8d-115">DateTimeOffset</span></span>|<span data-ttu-id="a9f8d-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a9f8d-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a9f8d-118">id</span><span class="sxs-lookup"><span data-stu-id="a9f8d-118">id</span></span>|<span data-ttu-id="a9f8d-119">String</span><span class="sxs-lookup"><span data-stu-id="a9f8d-119">String</span></span>| <span data-ttu-id="a9f8d-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9f8d-120">Read-only.</span></span>|
|<span data-ttu-id="a9f8d-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f8d-121">lastModifiedDateTime</span></span>|<span data-ttu-id="a9f8d-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f8d-122">DateTimeOffset</span></span>|<span data-ttu-id="a9f8d-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a9f8d-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9f8d-125">Relações</span><span class="sxs-lookup"><span data-stu-id="a9f8d-125">Relationships</span></span>
<span data-ttu-id="a9f8d-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9f8d-126">None</span></span>


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
