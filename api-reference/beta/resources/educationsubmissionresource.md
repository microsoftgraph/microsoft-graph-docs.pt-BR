---
title: tipo de recurso educationSubmissionResource
description: 'Um wrapper em torno de um recurso para uso em um envio. O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 329bab18d90412ec8cc06b12106e0be4f1b46935
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979559"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="d01fb-104">tipo de recurso educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d01fb-104">educationSubmissionResource resource type</span></span>

<span data-ttu-id="d01fb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d01fb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d01fb-106">Um wrapper em torno de um recurso para uso em um envio.</span><span class="sxs-lookup"><span data-stu-id="d01fb-106">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="d01fb-107">O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d01fb-107">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="d01fb-108">Methods</span><span class="sxs-lookup"><span data-stu-id="d01fb-108">Methods</span></span>

| <span data-ttu-id="d01fb-109">Método</span><span class="sxs-lookup"><span data-stu-id="d01fb-109">Method</span></span>           | <span data-ttu-id="d01fb-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d01fb-110">Return Type</span></span>    |<span data-ttu-id="d01fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d01fb-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d01fb-112">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d01fb-112">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="d01fb-113">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d01fb-113">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="d01fb-114">Ler propriedades e relações de um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="d01fb-114">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="d01fb-115">Delete</span><span class="sxs-lookup"><span data-stu-id="d01fb-115">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="d01fb-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d01fb-116">None</span></span> |<span data-ttu-id="d01fb-117">Excluir um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="d01fb-117">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d01fb-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d01fb-118">Properties</span></span>
| <span data-ttu-id="d01fb-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d01fb-119">Property</span></span>     | <span data-ttu-id="d01fb-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d01fb-120">Type</span></span>   |<span data-ttu-id="d01fb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d01fb-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d01fb-122">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="d01fb-122">assignmentResourceUrl</span></span>|<span data-ttu-id="d01fb-123">String</span><span class="sxs-lookup"><span data-stu-id="d01fb-123">String</span></span>|<span data-ttu-id="d01fb-124">Ponteiro para a atribuição da qual este recurso foi copiado.</span><span class="sxs-lookup"><span data-stu-id="d01fb-124">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="d01fb-125">Se isso for nulo, o aluno carregou o recurso.</span><span class="sxs-lookup"><span data-stu-id="d01fb-125">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="d01fb-126">id</span><span class="sxs-lookup"><span data-stu-id="d01fb-126">id</span></span>|<span data-ttu-id="d01fb-127">String</span><span class="sxs-lookup"><span data-stu-id="d01fb-127">String</span></span>| <span data-ttu-id="d01fb-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d01fb-128">Read-only.</span></span>|
|<span data-ttu-id="d01fb-129">recurso</span><span class="sxs-lookup"><span data-stu-id="d01fb-129">resource</span></span>|[<span data-ttu-id="d01fb-130">educationResource</span><span class="sxs-lookup"><span data-stu-id="d01fb-130">educationResource</span></span>](educationresource.md)|<span data-ttu-id="d01fb-131">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="d01fb-131">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d01fb-132">Relações</span><span class="sxs-lookup"><span data-stu-id="d01fb-132">Relationships</span></span>
<span data-ttu-id="d01fb-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d01fb-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d01fb-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d01fb-134">JSON representation</span></span>

<span data-ttu-id="d01fb-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d01fb-135">The following is a JSON representation of the resource.</span></span>

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


