---
title: recurso de onenoteEntityHierarchyModel
description: Este é um tipo de base para entidades do OneNote.
author: Jewan-microsoft
ms.openlocfilehash: a142e9206aefbb118f21b2f1a85d00cbc4a3a315
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362017"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="e7596-103">recurso de onenoteEntityHierarchyModel</span><span class="sxs-lookup"><span data-stu-id="e7596-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="e7596-104">Este é um tipo de base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e7596-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7596-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7596-105">JSON representation</span></span>

<span data-ttu-id="e7596-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7596-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}-->

```json
{
  "displayName": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="e7596-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7596-107">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="e7596-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7596-108">Properties</span></span>
| <span data-ttu-id="e7596-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7596-109">Property</span></span>     | <span data-ttu-id="e7596-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7596-110">Type</span></span>   |<span data-ttu-id="e7596-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7596-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7596-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e7596-112">displayName</span></span>|<span data-ttu-id="e7596-113">String</span><span class="sxs-lookup"><span data-stu-id="e7596-113">String</span></span>|<span data-ttu-id="e7596-114">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="e7596-114">The name of the notebook.</span></span>|
|<span data-ttu-id="e7596-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="e7596-115">createdBy</span></span>|[<span data-ttu-id="e7596-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="e7596-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="e7596-p101">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7596-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e7596-119">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e7596-119">lastModifiedBy</span></span>|[<span data-ttu-id="e7596-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="e7596-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="e7596-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7596-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e7596-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7596-123">lastModifiedDateTime</span></span>|<span data-ttu-id="e7596-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7596-124">DateTimeOffset</span></span>|<span data-ttu-id="e7596-p103">A data e hora da última modificação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7596-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->