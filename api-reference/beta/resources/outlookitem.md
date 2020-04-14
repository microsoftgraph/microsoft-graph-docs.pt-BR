---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 88436021375c85e85fc009611b2279705801ad12
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463238"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="a0222-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="a0222-103">outlookItem resource type</span></span>

<span data-ttu-id="a0222-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0222-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="a0222-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0222-105">JSON representation</span></span>

<span data-ttu-id="a0222-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a0222-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a0222-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0222-107">Properties</span></span>
| <span data-ttu-id="a0222-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0222-108">Property</span></span>     | <span data-ttu-id="a0222-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0222-109">Type</span></span>   |<span data-ttu-id="a0222-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0222-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0222-111">categories</span><span class="sxs-lookup"><span data-stu-id="a0222-111">categories</span></span>|<span data-ttu-id="a0222-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0222-112">String collection</span></span>||
|<span data-ttu-id="a0222-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="a0222-113">changeKey</span></span>|<span data-ttu-id="a0222-114">String</span><span class="sxs-lookup"><span data-stu-id="a0222-114">String</span></span>||
|<span data-ttu-id="a0222-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0222-115">createdDateTime</span></span>|<span data-ttu-id="a0222-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0222-116">DateTimeOffset</span></span>|<span data-ttu-id="a0222-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a0222-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a0222-119">id</span><span class="sxs-lookup"><span data-stu-id="a0222-119">id</span></span>|<span data-ttu-id="a0222-120">String</span><span class="sxs-lookup"><span data-stu-id="a0222-120">String</span></span>| <span data-ttu-id="a0222-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a0222-121">Read-only.</span></span>|
|<span data-ttu-id="a0222-122">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0222-122">lastModifiedDateTime</span></span>|<span data-ttu-id="a0222-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0222-123">DateTimeOffset</span></span>|<span data-ttu-id="a0222-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a0222-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0222-126">Relações</span><span class="sxs-lookup"><span data-stu-id="a0222-126">Relationships</span></span>
<span data-ttu-id="a0222-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0222-127">None</span></span>


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
