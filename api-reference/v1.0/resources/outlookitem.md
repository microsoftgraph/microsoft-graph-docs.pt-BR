---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
ms.openlocfilehash: 5f81598b62d2b47230f4a7ce16d17b8056bc9874
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004220"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="aea6c-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="aea6c-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="aea6c-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aea6c-104">JSON representation</span></span>

<span data-ttu-id="aea6c-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="aea6c-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="aea6c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aea6c-106">Properties</span></span>
| <span data-ttu-id="aea6c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aea6c-107">Property</span></span>     | <span data-ttu-id="aea6c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="aea6c-108">Type</span></span>   |<span data-ttu-id="aea6c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aea6c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aea6c-110">categories</span><span class="sxs-lookup"><span data-stu-id="aea6c-110">categories</span></span>|<span data-ttu-id="aea6c-111">String collection</span><span class="sxs-lookup"><span data-stu-id="aea6c-111">String collection</span></span>|<span data-ttu-id="aea6c-112">As categorias associadas ao item</span><span class="sxs-lookup"><span data-stu-id="aea6c-112">The categories associated with the item</span></span>|
|<span data-ttu-id="aea6c-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="aea6c-113">changeKey</span></span>|<span data-ttu-id="aea6c-114">String</span><span class="sxs-lookup"><span data-stu-id="aea6c-114">String</span></span>|<span data-ttu-id="aea6c-115">Identifica a versão do item.</span><span class="sxs-lookup"><span data-stu-id="aea6c-115">Identifies the version of the item.</span></span> <span data-ttu-id="aea6c-116">Toda vez que o item for alterado, changeKey também é alterado.</span><span class="sxs-lookup"><span data-stu-id="aea6c-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="aea6c-117">Isso permite que o Exchange para aplicar as alterações para a versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="aea6c-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="aea6c-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aea6c-118">Read-only.</span></span>|
|<span data-ttu-id="aea6c-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aea6c-119">createdDateTime</span></span>|<span data-ttu-id="aea6c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aea6c-120">DateTimeOffset</span></span>|<span data-ttu-id="aea6c-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="aea6c-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="aea6c-123">id</span><span class="sxs-lookup"><span data-stu-id="aea6c-123">id</span></span>|<span data-ttu-id="aea6c-124">String</span><span class="sxs-lookup"><span data-stu-id="aea6c-124">String</span></span>| <span data-ttu-id="aea6c-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aea6c-125">Read-only.</span></span>|
|<span data-ttu-id="aea6c-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aea6c-126">lastModifiedDateTime</span></span>|<span data-ttu-id="aea6c-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aea6c-127">DateTimeOffset</span></span>|<span data-ttu-id="aea6c-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="aea6c-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="aea6c-130">Relações</span><span class="sxs-lookup"><span data-stu-id="aea6c-130">Relationships</span></span>
<span data-ttu-id="aea6c-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aea6c-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
