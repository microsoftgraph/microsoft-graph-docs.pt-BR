---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 37a9d548e0eac3d07a66ca4b28c243c076a743bb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721534"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="a095b-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="a095b-103">outlookItem resource type</span></span>

<span data-ttu-id="a095b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a095b-104">Namespace: microsoft.graph</span></span>



## <a name="json-representation"></a><span data-ttu-id="a095b-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a095b-105">JSON representation</span></span>

<span data-ttu-id="a095b-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a095b-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a095b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a095b-107">Properties</span></span>
| <span data-ttu-id="a095b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a095b-108">Property</span></span>     | <span data-ttu-id="a095b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a095b-109">Type</span></span>   |<span data-ttu-id="a095b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a095b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a095b-111">Categorias</span><span class="sxs-lookup"><span data-stu-id="a095b-111">categories</span></span>|<span data-ttu-id="a095b-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a095b-112">String collection</span></span>|<span data-ttu-id="a095b-113">As categorias associadas ao item</span><span class="sxs-lookup"><span data-stu-id="a095b-113">The categories associated with the item</span></span>|
|<span data-ttu-id="a095b-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="a095b-114">changeKey</span></span>|<span data-ttu-id="a095b-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a095b-115">String</span></span>|<span data-ttu-id="a095b-116">Identifica a versão do item.</span><span class="sxs-lookup"><span data-stu-id="a095b-116">Identifies the version of the item.</span></span> <span data-ttu-id="a095b-117">Sempre que o item for alterado, changeKey também será alterado.</span><span class="sxs-lookup"><span data-stu-id="a095b-117">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="a095b-118">Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="a095b-118">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="a095b-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a095b-119">Read-only.</span></span>|
|<span data-ttu-id="a095b-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a095b-120">createdDateTime</span></span>|<span data-ttu-id="a095b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a095b-121">DateTimeOffset</span></span>|<span data-ttu-id="a095b-122">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a095b-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a095b-123">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a095b-123">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a095b-124">id</span><span class="sxs-lookup"><span data-stu-id="a095b-124">id</span></span>|<span data-ttu-id="a095b-125">String</span><span class="sxs-lookup"><span data-stu-id="a095b-125">String</span></span>| <span data-ttu-id="a095b-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a095b-126">Read-only.</span></span>|
|<span data-ttu-id="a095b-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a095b-127">lastModifiedDateTime</span></span>|<span data-ttu-id="a095b-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a095b-128">DateTimeOffset</span></span>|<span data-ttu-id="a095b-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a095b-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a095b-130">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a095b-130">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a095b-131">Relações</span><span class="sxs-lookup"><span data-stu-id="a095b-131">Relationships</span></span>
<span data-ttu-id="a095b-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a095b-132">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

