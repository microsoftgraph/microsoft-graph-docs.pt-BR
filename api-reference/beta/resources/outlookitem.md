---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8a44f9a2e568991c6803ebf72baf5f712f39ba64
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528288"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="11c56-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="11c56-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="11c56-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11c56-104">JSON representation</span></span>

<span data-ttu-id="11c56-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="11c56-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookitem"
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
## <a name="properties"></a><span data-ttu-id="11c56-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11c56-106">Properties</span></span>
| <span data-ttu-id="11c56-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11c56-107">Property</span></span>     | <span data-ttu-id="11c56-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="11c56-108">Type</span></span>   |<span data-ttu-id="11c56-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="11c56-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11c56-110">categories</span><span class="sxs-lookup"><span data-stu-id="11c56-110">categories</span></span>|<span data-ttu-id="11c56-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="11c56-111">String collection</span></span>||
|<span data-ttu-id="11c56-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="11c56-112">changeKey</span></span>|<span data-ttu-id="11c56-113">String</span><span class="sxs-lookup"><span data-stu-id="11c56-113">String</span></span>||
|<span data-ttu-id="11c56-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11c56-114">createdDateTime</span></span>|<span data-ttu-id="11c56-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11c56-115">DateTimeOffset</span></span>|<span data-ttu-id="11c56-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="11c56-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="11c56-118">id</span><span class="sxs-lookup"><span data-stu-id="11c56-118">id</span></span>|<span data-ttu-id="11c56-119">String</span><span class="sxs-lookup"><span data-stu-id="11c56-119">String</span></span>| <span data-ttu-id="11c56-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11c56-120">Read-only.</span></span>|
|<span data-ttu-id="11c56-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11c56-121">lastModifiedDateTime</span></span>|<span data-ttu-id="11c56-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11c56-122">DateTimeOffset</span></span>|<span data-ttu-id="11c56-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="11c56-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="11c56-125">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="11c56-125">Relationships</span></span>
<span data-ttu-id="11c56-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11c56-126">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
