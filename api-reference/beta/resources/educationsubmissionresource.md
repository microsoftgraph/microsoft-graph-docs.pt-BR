---
title: tipo de recurso de educationSubmissionResource
description: 'Um wrapper em torno de um recurso para uso em um envio. O wrapper adiciona um ponteiro para o recurso de atribuição, se isso foi copiado da atribuição.  '
author: dipakboyed
ms.openlocfilehash: bfbf2f522106f5a1e2033898cbb2702223d3e241
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361555"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="3d7f7-104">tipo de recurso de educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="3d7f7-104">educationSubmissionResource resource type</span></span>

> <span data-ttu-id="3d7f7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3d7f7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d7f7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3d7f7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d7f7-107">Um wrapper em torno de um recurso para uso em um envio.</span><span class="sxs-lookup"><span data-stu-id="3d7f7-107">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="3d7f7-108">O wrapper adiciona um ponteiro para o recurso de atribuição, se isso foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="3d7f7-108">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="3d7f7-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="3d7f7-109">Methods</span></span>

| <span data-ttu-id="3d7f7-110">Método</span><span class="sxs-lookup"><span data-stu-id="3d7f7-110">Method</span></span>           | <span data-ttu-id="3d7f7-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3d7f7-111">Return Type</span></span>    |<span data-ttu-id="3d7f7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d7f7-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3d7f7-113">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="3d7f7-113">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="3d7f7-114">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="3d7f7-114">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="3d7f7-115">Leia as propriedades e os relacionamentos de um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="3d7f7-115">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="3d7f7-116">Delete</span><span class="sxs-lookup"><span data-stu-id="3d7f7-116">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="3d7f7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d7f7-117">None</span></span> |<span data-ttu-id="3d7f7-118">Exclua um objeto **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="3d7f7-118">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3d7f7-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d7f7-119">Properties</span></span>
| <span data-ttu-id="3d7f7-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d7f7-120">Property</span></span>     | <span data-ttu-id="3d7f7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d7f7-121">Type</span></span>   |<span data-ttu-id="3d7f7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d7f7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d7f7-123">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="3d7f7-123">assignmentResourceUrl</span></span>|<span data-ttu-id="3d7f7-124">String</span><span class="sxs-lookup"><span data-stu-id="3d7f7-124">String</span></span>|<span data-ttu-id="3d7f7-125">Ponteiro para a atribuição do qual este recurso foi copiado.</span><span class="sxs-lookup"><span data-stu-id="3d7f7-125">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="3d7f7-126">Se for nulo, o aluno carregado o recurso.</span><span class="sxs-lookup"><span data-stu-id="3d7f7-126">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="3d7f7-127">id</span><span class="sxs-lookup"><span data-stu-id="3d7f7-127">id</span></span>|<span data-ttu-id="3d7f7-128">String</span><span class="sxs-lookup"><span data-stu-id="3d7f7-128">String</span></span>| <span data-ttu-id="3d7f7-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d7f7-129">Read-only.</span></span>|
|<span data-ttu-id="3d7f7-130">recurso</span><span class="sxs-lookup"><span data-stu-id="3d7f7-130">resource</span></span>|[<span data-ttu-id="3d7f7-131">educationResource</span><span class="sxs-lookup"><span data-stu-id="3d7f7-131">educationResource</span></span>](educationresource.md)|<span data-ttu-id="3d7f7-132">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="3d7f7-132">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d7f7-133">Relações</span><span class="sxs-lookup"><span data-stu-id="3d7f7-133">Relationships</span></span>
<span data-ttu-id="3d7f7-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d7f7-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3d7f7-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d7f7-135">JSON representation</span></span>

<span data-ttu-id="3d7f7-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d7f7-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->