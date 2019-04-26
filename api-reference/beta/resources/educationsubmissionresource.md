---
title: tipo de recurso educationSubmissionResource
description: 'Um wrapper em torno de um recurso para uso em um envio. O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b96607a0d37a3ec8af0f6ff0bad61215d6e9008c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340568"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="316fe-104">tipo de recurso educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="316fe-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="316fe-105">Um wrapper em torno de um recurso para uso em um envio.</span><span class="sxs-lookup"><span data-stu-id="316fe-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="316fe-106">O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="316fe-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="316fe-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="316fe-107">Methods</span></span>

| <span data-ttu-id="316fe-108">Método</span><span class="sxs-lookup"><span data-stu-id="316fe-108">Method</span></span>           | <span data-ttu-id="316fe-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="316fe-109">Return Type</span></span>    |<span data-ttu-id="316fe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="316fe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="316fe-111">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="316fe-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="316fe-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="316fe-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="316fe-113">Ler propriedades e relações de um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="316fe-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="316fe-114">Delete</span><span class="sxs-lookup"><span data-stu-id="316fe-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="316fe-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="316fe-115">None</span></span> |<span data-ttu-id="316fe-116">Excluir um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="316fe-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="316fe-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="316fe-117">Properties</span></span>
| <span data-ttu-id="316fe-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="316fe-118">Property</span></span>     | <span data-ttu-id="316fe-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="316fe-119">Type</span></span>   |<span data-ttu-id="316fe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="316fe-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="316fe-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="316fe-121">assignmentResourceUrl</span></span>|<span data-ttu-id="316fe-122">String</span><span class="sxs-lookup"><span data-stu-id="316fe-122">String</span></span>|<span data-ttu-id="316fe-123">Ponteiro para a atribuição da qual este recurso foi copiado.</span><span class="sxs-lookup"><span data-stu-id="316fe-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="316fe-124">Se isso for nulo, o aluno carregou o recurso.</span><span class="sxs-lookup"><span data-stu-id="316fe-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="316fe-125">id</span><span class="sxs-lookup"><span data-stu-id="316fe-125">id</span></span>|<span data-ttu-id="316fe-126">String</span><span class="sxs-lookup"><span data-stu-id="316fe-126">String</span></span>| <span data-ttu-id="316fe-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="316fe-127">Read-only.</span></span>|
|<span data-ttu-id="316fe-128">recurso</span><span class="sxs-lookup"><span data-stu-id="316fe-128">resource</span></span>|[<span data-ttu-id="316fe-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="316fe-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="316fe-130">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="316fe-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="316fe-131">Relações</span><span class="sxs-lookup"><span data-stu-id="316fe-131">Relationships</span></span>
<span data-ttu-id="316fe-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="316fe-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="316fe-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="316fe-133">JSON representation</span></span>

<span data-ttu-id="316fe-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="316fe-134">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
