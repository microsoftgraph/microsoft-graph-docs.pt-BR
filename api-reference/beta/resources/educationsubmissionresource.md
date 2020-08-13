---
title: tipo de recurso educationSubmissionResource
description: 'Um wrapper em torno de um recurso para uso em um envio. O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 876a490c3dfcf69eb993d1ba18868e2fc5a62fa8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500636"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="756ca-104">tipo de recurso educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="756ca-104">educationSubmissionResource resource type</span></span>

<span data-ttu-id="756ca-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="756ca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="756ca-106">Um wrapper em torno de um recurso para uso em um envio.</span><span class="sxs-lookup"><span data-stu-id="756ca-106">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="756ca-107">O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="756ca-107">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="756ca-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="756ca-108">Methods</span></span>

| <span data-ttu-id="756ca-109">Método</span><span class="sxs-lookup"><span data-stu-id="756ca-109">Method</span></span>           | <span data-ttu-id="756ca-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="756ca-110">Return Type</span></span>    |<span data-ttu-id="756ca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="756ca-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="756ca-112">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="756ca-112">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="756ca-113">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="756ca-113">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="756ca-114">Ler propriedades e relações de um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="756ca-114">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="756ca-115">Delete</span><span class="sxs-lookup"><span data-stu-id="756ca-115">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="756ca-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="756ca-116">None</span></span> |<span data-ttu-id="756ca-117">Excluir um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="756ca-117">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="756ca-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="756ca-118">Properties</span></span>
| <span data-ttu-id="756ca-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="756ca-119">Property</span></span>     | <span data-ttu-id="756ca-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="756ca-120">Type</span></span>   |<span data-ttu-id="756ca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="756ca-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="756ca-122">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="756ca-122">assignmentResourceUrl</span></span>|<span data-ttu-id="756ca-123">String</span><span class="sxs-lookup"><span data-stu-id="756ca-123">String</span></span>|<span data-ttu-id="756ca-124">Ponteiro para a atribuição da qual este recurso foi copiado.</span><span class="sxs-lookup"><span data-stu-id="756ca-124">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="756ca-125">Se isso for nulo, o aluno carregou o recurso.</span><span class="sxs-lookup"><span data-stu-id="756ca-125">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="756ca-126">id</span><span class="sxs-lookup"><span data-stu-id="756ca-126">id</span></span>|<span data-ttu-id="756ca-127">String</span><span class="sxs-lookup"><span data-stu-id="756ca-127">String</span></span>| <span data-ttu-id="756ca-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756ca-128">Read-only.</span></span>|
|<span data-ttu-id="756ca-129">recurso</span><span class="sxs-lookup"><span data-stu-id="756ca-129">resource</span></span>|[<span data-ttu-id="756ca-130">educationResource</span><span class="sxs-lookup"><span data-stu-id="756ca-130">educationResource</span></span>](educationresource.md)|<span data-ttu-id="756ca-131">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="756ca-131">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="756ca-132">Relações</span><span class="sxs-lookup"><span data-stu-id="756ca-132">Relationships</span></span>
<span data-ttu-id="756ca-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="756ca-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="756ca-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="756ca-134">JSON representation</span></span>

<span data-ttu-id="756ca-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="756ca-135">The following is a JSON representation of the resource.</span></span>

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
