---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 284a53ab713be49d29c19a6d4b69b3b51047977f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137358"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="fe276-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="fe276-103">outlookItem resource type</span></span>

<span data-ttu-id="fe276-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe276-104">Namespace: microsoft.graph</span></span>



## <a name="json-representation"></a><span data-ttu-id="fe276-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe276-105">JSON representation</span></span>

<span data-ttu-id="fe276-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fe276-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="fe276-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe276-107">Properties</span></span>
| <span data-ttu-id="fe276-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe276-108">Property</span></span>     | <span data-ttu-id="fe276-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe276-109">Type</span></span>   |<span data-ttu-id="fe276-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe276-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe276-111">categories</span><span class="sxs-lookup"><span data-stu-id="fe276-111">categories</span></span>|<span data-ttu-id="fe276-112">String collection</span><span class="sxs-lookup"><span data-stu-id="fe276-112">String collection</span></span>|<span data-ttu-id="fe276-113">As categorias associadas ao item</span><span class="sxs-lookup"><span data-stu-id="fe276-113">The categories associated with the item</span></span>|
|<span data-ttu-id="fe276-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="fe276-114">changeKey</span></span>|<span data-ttu-id="fe276-115">String</span><span class="sxs-lookup"><span data-stu-id="fe276-115">String</span></span>|<span data-ttu-id="fe276-116">Identifica a versão do item.</span><span class="sxs-lookup"><span data-stu-id="fe276-116">Identifies the version of the item.</span></span> <span data-ttu-id="fe276-117">Toda vez que o item é alterado, changeKey também muda.</span><span class="sxs-lookup"><span data-stu-id="fe276-117">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="fe276-118">Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="fe276-118">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="fe276-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fe276-119">Read-only.</span></span>|
|<span data-ttu-id="fe276-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe276-120">createdDateTime</span></span>|<span data-ttu-id="fe276-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe276-121">DateTimeOffset</span></span>|<span data-ttu-id="fe276-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fe276-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fe276-124">id</span><span class="sxs-lookup"><span data-stu-id="fe276-124">id</span></span>|<span data-ttu-id="fe276-125">String</span><span class="sxs-lookup"><span data-stu-id="fe276-125">String</span></span>| <span data-ttu-id="fe276-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fe276-126">Read-only.</span></span>|
|<span data-ttu-id="fe276-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe276-127">lastModifiedDateTime</span></span>|<span data-ttu-id="fe276-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe276-128">DateTimeOffset</span></span>|<span data-ttu-id="fe276-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fe276-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe276-131">Relações</span><span class="sxs-lookup"><span data-stu-id="fe276-131">Relationships</span></span>
<span data-ttu-id="fe276-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe276-132">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

