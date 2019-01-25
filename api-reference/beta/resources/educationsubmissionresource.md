---
title: tipo de recurso de educationSubmissionResource
description: 'Um wrapper em torno de um recurso para uso em um envio. O wrapper adiciona um ponteiro para o recurso de atribuição, se isso foi copiado da atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ef231de49d3871ec877c279b4e77585343e1a85e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522074"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="b6a8b-104">tipo de recurso de educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="b6a8b-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6a8b-105">Um wrapper em torno de um recurso para uso em um envio.</span><span class="sxs-lookup"><span data-stu-id="b6a8b-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="b6a8b-106">O wrapper adiciona um ponteiro para o recurso de atribuição, se isso foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="b6a8b-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="b6a8b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b6a8b-107">Methods</span></span>

| <span data-ttu-id="b6a8b-108">Método</span><span class="sxs-lookup"><span data-stu-id="b6a8b-108">Method</span></span>           | <span data-ttu-id="b6a8b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b6a8b-109">Return Type</span></span>    |<span data-ttu-id="b6a8b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6a8b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6a8b-111">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="b6a8b-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="b6a8b-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="b6a8b-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="b6a8b-113">Leia as propriedades e os relacionamentos de um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="b6a8b-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="b6a8b-114">Delete</span><span class="sxs-lookup"><span data-stu-id="b6a8b-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="b6a8b-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6a8b-115">None</span></span> |<span data-ttu-id="b6a8b-116">Exclua um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="b6a8b-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6a8b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6a8b-117">Properties</span></span>
| <span data-ttu-id="b6a8b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6a8b-118">Property</span></span>     | <span data-ttu-id="b6a8b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6a8b-119">Type</span></span>   |<span data-ttu-id="b6a8b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6a8b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6a8b-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="b6a8b-121">assignmentResourceUrl</span></span>|<span data-ttu-id="b6a8b-122">String</span><span class="sxs-lookup"><span data-stu-id="b6a8b-122">String</span></span>|<span data-ttu-id="b6a8b-123">Ponteiro para a atribuição do qual este recurso foi copiado.</span><span class="sxs-lookup"><span data-stu-id="b6a8b-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="b6a8b-124">Se for nulo, o aluno carregado o recurso.</span><span class="sxs-lookup"><span data-stu-id="b6a8b-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="b6a8b-125">id</span><span class="sxs-lookup"><span data-stu-id="b6a8b-125">id</span></span>|<span data-ttu-id="b6a8b-126">String</span><span class="sxs-lookup"><span data-stu-id="b6a8b-126">String</span></span>| <span data-ttu-id="b6a8b-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6a8b-127">Read-only.</span></span>|
|<span data-ttu-id="b6a8b-128">recurso</span><span class="sxs-lookup"><span data-stu-id="b6a8b-128">resource</span></span>|[<span data-ttu-id="b6a8b-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="b6a8b-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="b6a8b-130">Objeto Resource</span><span class="sxs-lookup"><span data-stu-id="b6a8b-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6a8b-131">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="b6a8b-131">Relationships</span></span>
<span data-ttu-id="b6a8b-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6a8b-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b6a8b-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6a8b-133">JSON representation</span></span>

<span data-ttu-id="b6a8b-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6a8b-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
