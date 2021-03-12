---
title: Recurso onenoteEntityHierarchyModel
description: Esse é um tipo base para entidades do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 2ddad970ead6c8bd575267f04266426e54a66568
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720855"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="4a7b0-103">Recurso onenoteEntityHierarchyModel</span><span class="sxs-lookup"><span data-stu-id="4a7b0-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="4a7b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a7b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a7b0-105">Esse é um tipo base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="4a7b0-105">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a7b0-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a7b0-106">JSON representation</span></span>

<span data-ttu-id="4a7b0-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a7b0-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="4a7b0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a7b0-108">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="4a7b0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a7b0-109">Properties</span></span>
| <span data-ttu-id="4a7b0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a7b0-110">Property</span></span>     | <span data-ttu-id="4a7b0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a7b0-111">Type</span></span>   |<span data-ttu-id="4a7b0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a7b0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a7b0-113">displayName</span><span class="sxs-lookup"><span data-stu-id="4a7b0-113">displayName</span></span>|<span data-ttu-id="4a7b0-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a7b0-114">String</span></span>|<span data-ttu-id="4a7b0-115">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="4a7b0-115">The name of the notebook.</span></span>|
|<span data-ttu-id="4a7b0-116">createdBy</span><span class="sxs-lookup"><span data-stu-id="4a7b0-116">createdBy</span></span>|[<span data-ttu-id="4a7b0-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="4a7b0-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="4a7b0-p101">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a7b0-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="4a7b0-120">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4a7b0-120">lastModifiedBy</span></span>|[<span data-ttu-id="4a7b0-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="4a7b0-121">identitySet</span></span>](identityset.md)|<span data-ttu-id="4a7b0-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a7b0-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="4a7b0-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a7b0-124">lastModifiedDateTime</span></span>|<span data-ttu-id="4a7b0-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a7b0-125">DateTimeOffset</span></span>|<span data-ttu-id="4a7b0-126">A data e hora da última modificação do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="4a7b0-126">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="4a7b0-127">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4a7b0-127">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4a7b0-128">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4a7b0-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="4a7b0-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a7b0-129">Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

