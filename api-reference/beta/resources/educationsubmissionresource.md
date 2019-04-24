---
title: tipo de recurso educationSubmissionResource
description: 'Um wrapper em torno de um recurso para uso em um envio. O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ef231de49d3871ec877c279b4e77585343e1a85e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507074"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="727a3-104">tipo de recurso educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="727a3-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="727a3-105">Um wrapper em torno de um recurso para uso em um envio.</span><span class="sxs-lookup"><span data-stu-id="727a3-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="727a3-106">O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="727a3-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="727a3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="727a3-107">Methods</span></span>

| <span data-ttu-id="727a3-108">Método</span><span class="sxs-lookup"><span data-stu-id="727a3-108">Method</span></span>           | <span data-ttu-id="727a3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="727a3-109">Return Type</span></span>    |<span data-ttu-id="727a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="727a3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="727a3-111">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="727a3-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="727a3-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="727a3-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="727a3-113">Ler propriedades e relações de um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="727a3-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="727a3-114">Excluir</span><span class="sxs-lookup"><span data-stu-id="727a3-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="727a3-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="727a3-115">None</span></span> |<span data-ttu-id="727a3-116">Excluir um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="727a3-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="727a3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="727a3-117">Properties</span></span>
| <span data-ttu-id="727a3-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="727a3-118">Property</span></span>     | <span data-ttu-id="727a3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="727a3-119">Type</span></span>   |<span data-ttu-id="727a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="727a3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="727a3-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="727a3-121">assignmentResourceUrl</span></span>|<span data-ttu-id="727a3-122">String</span><span class="sxs-lookup"><span data-stu-id="727a3-122">String</span></span>|<span data-ttu-id="727a3-123">Ponteiro para a atribuição da qual este recurso foi copiado.</span><span class="sxs-lookup"><span data-stu-id="727a3-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="727a3-124">Se isso for nulo, o aluno carregou o recurso.</span><span class="sxs-lookup"><span data-stu-id="727a3-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="727a3-125">id</span><span class="sxs-lookup"><span data-stu-id="727a3-125">id</span></span>|<span data-ttu-id="727a3-126">String</span><span class="sxs-lookup"><span data-stu-id="727a3-126">String</span></span>| <span data-ttu-id="727a3-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="727a3-127">Read-only.</span></span>|
|<span data-ttu-id="727a3-128">recurso</span><span class="sxs-lookup"><span data-stu-id="727a3-128">resource</span></span>|[<span data-ttu-id="727a3-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="727a3-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="727a3-130">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="727a3-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="727a3-131">Relações</span><span class="sxs-lookup"><span data-stu-id="727a3-131">Relationships</span></span>
<span data-ttu-id="727a3-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="727a3-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="727a3-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="727a3-133">JSON representation</span></span>

<span data-ttu-id="727a3-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="727a3-134">The following is a JSON representation of the resource.</span></span>

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
