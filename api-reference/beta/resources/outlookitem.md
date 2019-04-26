---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b2c43d81d045ee6b563e7ae81f8fe6fab56bdf83
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341845"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="d9bbf-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="d9bbf-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="d9bbf-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9bbf-104">JSON representation</span></span>

<span data-ttu-id="d9bbf-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d9bbf-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d9bbf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9bbf-106">Properties</span></span>
| <span data-ttu-id="d9bbf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9bbf-107">Property</span></span>     | <span data-ttu-id="d9bbf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9bbf-108">Type</span></span>   |<span data-ttu-id="d9bbf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9bbf-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9bbf-110">categories</span><span class="sxs-lookup"><span data-stu-id="d9bbf-110">categories</span></span>|<span data-ttu-id="d9bbf-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9bbf-111">String collection</span></span>||
|<span data-ttu-id="d9bbf-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="d9bbf-112">changeKey</span></span>|<span data-ttu-id="d9bbf-113">String</span><span class="sxs-lookup"><span data-stu-id="d9bbf-113">String</span></span>||
|<span data-ttu-id="d9bbf-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9bbf-114">createdDateTime</span></span>|<span data-ttu-id="d9bbf-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9bbf-115">DateTimeOffset</span></span>|<span data-ttu-id="d9bbf-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d9bbf-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d9bbf-118">id</span><span class="sxs-lookup"><span data-stu-id="d9bbf-118">id</span></span>|<span data-ttu-id="d9bbf-119">String</span><span class="sxs-lookup"><span data-stu-id="d9bbf-119">String</span></span>| <span data-ttu-id="d9bbf-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9bbf-120">Read-only.</span></span>|
|<span data-ttu-id="d9bbf-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9bbf-121">lastModifiedDateTime</span></span>|<span data-ttu-id="d9bbf-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9bbf-122">DateTimeOffset</span></span>|<span data-ttu-id="d9bbf-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d9bbf-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9bbf-125">Relações</span><span class="sxs-lookup"><span data-stu-id="d9bbf-125">Relationships</span></span>
<span data-ttu-id="d9bbf-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9bbf-126">None</span></span>


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
