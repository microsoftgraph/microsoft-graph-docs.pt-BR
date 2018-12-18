---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: angelgolfer-ms
ms.openlocfilehash: 750239156e6f4e2874783ae160a7018fb58e259d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332512"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="436d6-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="436d6-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="436d6-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="436d6-104">JSON representation</span></span>

<span data-ttu-id="436d6-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="436d6-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="436d6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="436d6-106">Properties</span></span>
| <span data-ttu-id="436d6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="436d6-107">Property</span></span>     | <span data-ttu-id="436d6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="436d6-108">Type</span></span>   |<span data-ttu-id="436d6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="436d6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="436d6-110">categories</span><span class="sxs-lookup"><span data-stu-id="436d6-110">categories</span></span>|<span data-ttu-id="436d6-111">String collection</span><span class="sxs-lookup"><span data-stu-id="436d6-111">String collection</span></span>|<span data-ttu-id="436d6-112">As categorias associadas ao item</span><span class="sxs-lookup"><span data-stu-id="436d6-112">The categories associated with the item</span></span>|
|<span data-ttu-id="436d6-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="436d6-113">changeKey</span></span>|<span data-ttu-id="436d6-114">String</span><span class="sxs-lookup"><span data-stu-id="436d6-114">String</span></span>|<span data-ttu-id="436d6-115">Identifica a versão do item.</span><span class="sxs-lookup"><span data-stu-id="436d6-115">Identifies the version of the item.</span></span> <span data-ttu-id="436d6-116">Toda vez que o item for alterado, changeKey também é alterado.</span><span class="sxs-lookup"><span data-stu-id="436d6-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="436d6-117">Isso permite que o Exchange para aplicar as alterações para a versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="436d6-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="436d6-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="436d6-118">Read-only.</span></span>|
|<span data-ttu-id="436d6-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="436d6-119">createdDateTime</span></span>|<span data-ttu-id="436d6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="436d6-120">DateTimeOffset</span></span>|<span data-ttu-id="436d6-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="436d6-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="436d6-123">id</span><span class="sxs-lookup"><span data-stu-id="436d6-123">id</span></span>|<span data-ttu-id="436d6-124">String</span><span class="sxs-lookup"><span data-stu-id="436d6-124">String</span></span>| <span data-ttu-id="436d6-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="436d6-125">Read-only.</span></span>|
|<span data-ttu-id="436d6-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="436d6-126">lastModifiedDateTime</span></span>|<span data-ttu-id="436d6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="436d6-127">DateTimeOffset</span></span>|<span data-ttu-id="436d6-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="436d6-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="436d6-130">Relações</span><span class="sxs-lookup"><span data-stu-id="436d6-130">Relationships</span></span>
<span data-ttu-id="436d6-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="436d6-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
