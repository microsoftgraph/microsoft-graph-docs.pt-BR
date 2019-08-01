---
title: recurso onenoteEntityHierarchyModel
description: Este é um tipo base para entidades do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: febe87c3c57612dae06e3a34a187399e6b94c55a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035823"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="3377d-103">recurso onenoteEntityHierarchyModel</span><span class="sxs-lookup"><span data-stu-id="3377d-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="3377d-104">Este é um tipo base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="3377d-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3377d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3377d-105">JSON representation</span></span>

<span data-ttu-id="3377d-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3377d-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3377d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3377d-107">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="3377d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3377d-108">Properties</span></span>
| <span data-ttu-id="3377d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3377d-109">Property</span></span>     | <span data-ttu-id="3377d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3377d-110">Type</span></span>   |<span data-ttu-id="3377d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3377d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3377d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3377d-112">displayName</span></span>|<span data-ttu-id="3377d-113">String</span><span class="sxs-lookup"><span data-stu-id="3377d-113">String</span></span>|<span data-ttu-id="3377d-114">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="3377d-114">The name of the notebook.</span></span>|
|<span data-ttu-id="3377d-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="3377d-115">createdBy</span></span>|[<span data-ttu-id="3377d-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="3377d-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="3377d-p101">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3377d-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="3377d-119">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3377d-119">lastModifiedBy</span></span>|[<span data-ttu-id="3377d-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="3377d-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="3377d-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3377d-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="3377d-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3377d-123">lastModifiedDateTime</span></span>|<span data-ttu-id="3377d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3377d-124">DateTimeOffset</span></span>|<span data-ttu-id="3377d-125">A data e hora da última modificação do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="3377d-125">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="3377d-126">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3377d-126">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3377d-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3377d-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3377d-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3377d-128">Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
