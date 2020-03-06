---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: aa5e4af03171029e8557e38d3a75062161435318
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534110"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="bbcbe-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="bbcbe-103">outlookItem resource type</span></span>

<span data-ttu-id="bbcbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbcbe-104">Namespace: microsoft.graph</span></span>



## <a name="json-representation"></a><span data-ttu-id="bbcbe-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbcbe-105">JSON representation</span></span>

<span data-ttu-id="bbcbe-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bbcbe-106">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
## <a name="properties"></a><span data-ttu-id="bbcbe-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbcbe-107">Properties</span></span>
| <span data-ttu-id="bbcbe-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbcbe-108">Property</span></span>     | <span data-ttu-id="bbcbe-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbcbe-109">Type</span></span>   |<span data-ttu-id="bbcbe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbcbe-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbcbe-111">categories</span><span class="sxs-lookup"><span data-stu-id="bbcbe-111">categories</span></span>|<span data-ttu-id="bbcbe-112">String collection</span><span class="sxs-lookup"><span data-stu-id="bbcbe-112">String collection</span></span>|<span data-ttu-id="bbcbe-113">As categorias associadas ao item</span><span class="sxs-lookup"><span data-stu-id="bbcbe-113">The categories associated with the item</span></span>|
|<span data-ttu-id="bbcbe-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="bbcbe-114">changeKey</span></span>|<span data-ttu-id="bbcbe-115">String</span><span class="sxs-lookup"><span data-stu-id="bbcbe-115">String</span></span>|<span data-ttu-id="bbcbe-116">Identifica a versão do item.</span><span class="sxs-lookup"><span data-stu-id="bbcbe-116">Identifies the version of the item.</span></span> <span data-ttu-id="bbcbe-117">Sempre que o item for alterado, changeKey também será alterado.</span><span class="sxs-lookup"><span data-stu-id="bbcbe-117">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="bbcbe-118">Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="bbcbe-118">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="bbcbe-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bbcbe-119">Read-only.</span></span>|
|<span data-ttu-id="bbcbe-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bbcbe-120">createdDateTime</span></span>|<span data-ttu-id="bbcbe-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbcbe-121">DateTimeOffset</span></span>|<span data-ttu-id="bbcbe-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bbcbe-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bbcbe-124">id</span><span class="sxs-lookup"><span data-stu-id="bbcbe-124">id</span></span>|<span data-ttu-id="bbcbe-125">String</span><span class="sxs-lookup"><span data-stu-id="bbcbe-125">String</span></span>| <span data-ttu-id="bbcbe-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bbcbe-126">Read-only.</span></span>|
|<span data-ttu-id="bbcbe-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbcbe-127">lastModifiedDateTime</span></span>|<span data-ttu-id="bbcbe-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbcbe-128">DateTimeOffset</span></span>|<span data-ttu-id="bbcbe-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bbcbe-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbcbe-131">Relações</span><span class="sxs-lookup"><span data-stu-id="bbcbe-131">Relationships</span></span>
<span data-ttu-id="bbcbe-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbcbe-132">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
