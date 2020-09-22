---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8b65b4fd8866cdde99460d42d39e40ef322b6278
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066268"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="b26b7-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="b26b7-103">outlookItem resource type</span></span>

<span data-ttu-id="b26b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b26b7-104">Namespace: microsoft.graph</span></span>



## <a name="json-representation"></a><span data-ttu-id="b26b7-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b26b7-105">JSON representation</span></span>

<span data-ttu-id="b26b7-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b26b7-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b26b7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b26b7-107">Properties</span></span>
| <span data-ttu-id="b26b7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b26b7-108">Property</span></span>     | <span data-ttu-id="b26b7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b26b7-109">Type</span></span>   |<span data-ttu-id="b26b7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b26b7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b26b7-111">Categorias</span><span class="sxs-lookup"><span data-stu-id="b26b7-111">categories</span></span>|<span data-ttu-id="b26b7-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b26b7-112">String collection</span></span>|<span data-ttu-id="b26b7-113">As categorias associadas ao item</span><span class="sxs-lookup"><span data-stu-id="b26b7-113">The categories associated with the item</span></span>|
|<span data-ttu-id="b26b7-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="b26b7-114">changeKey</span></span>|<span data-ttu-id="b26b7-115">String</span><span class="sxs-lookup"><span data-stu-id="b26b7-115">String</span></span>|<span data-ttu-id="b26b7-116">Identifica a versão do item.</span><span class="sxs-lookup"><span data-stu-id="b26b7-116">Identifies the version of the item.</span></span> <span data-ttu-id="b26b7-117">Sempre que o item for alterado, changeKey também será alterado.</span><span class="sxs-lookup"><span data-stu-id="b26b7-117">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="b26b7-118">Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="b26b7-118">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="b26b7-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b26b7-119">Read-only.</span></span>|
|<span data-ttu-id="b26b7-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b26b7-120">createdDateTime</span></span>|<span data-ttu-id="b26b7-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b26b7-121">DateTimeOffset</span></span>|<span data-ttu-id="b26b7-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b26b7-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b26b7-124">id</span><span class="sxs-lookup"><span data-stu-id="b26b7-124">id</span></span>|<span data-ttu-id="b26b7-125">String</span><span class="sxs-lookup"><span data-stu-id="b26b7-125">String</span></span>| <span data-ttu-id="b26b7-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b26b7-126">Read-only.</span></span>|
|<span data-ttu-id="b26b7-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b26b7-127">lastModifiedDateTime</span></span>|<span data-ttu-id="b26b7-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b26b7-128">DateTimeOffset</span></span>|<span data-ttu-id="b26b7-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b26b7-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="b26b7-131">Relações</span><span class="sxs-lookup"><span data-stu-id="b26b7-131">Relationships</span></span>
<span data-ttu-id="b26b7-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b26b7-132">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

