---
title: tipo de recurso educationAssignmentResource
description: Um objeto envoltório que armazena os recursos associados a uma atribuição. O wrapper adiciona a propriedade **distributeForStudentWork** e indica que este recurso irá
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 462433a24b8515146303505865b3d356d025d6c4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095545"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="9c876-104">tipo de recurso educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="9c876-104">educationAssignmentResource resource type</span></span>

<span data-ttu-id="9c876-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c876-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c876-106">Um objeto envoltório que armazena os recursos associados a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="9c876-106">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="9c876-107">O wrapper adiciona a propriedade **distributeForStudentWork** e indica que esse recurso será copiado para o envio do aluno.</span><span class="sxs-lookup"><span data-stu-id="9c876-107">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="9c876-108">Se o objeto não for copiado, cada aluno verá um link para o recurso na atribuição.</span><span class="sxs-lookup"><span data-stu-id="9c876-108">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="9c876-109">O aluno não poderá atualizar esse recurso.</span><span class="sxs-lookup"><span data-stu-id="9c876-109">The student will not be able to update this resource.</span></span> <span data-ttu-id="9c876-110">Este é um folheto do professor para o aluno com nada para ser ativado.</span><span class="sxs-lookup"><span data-stu-id="9c876-110">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="9c876-111">Se o recurso for distribuído, cada aluno receberá uma cópia desse recurso na lista de recursos do envio.</span><span class="sxs-lookup"><span data-stu-id="9c876-111">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="9c876-112">Cada aluno poderá modificar a cópia e enviá-la para a gradação.</span><span class="sxs-lookup"><span data-stu-id="9c876-112">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="9c876-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="9c876-113">Methods</span></span>

| <span data-ttu-id="9c876-114">Método</span><span class="sxs-lookup"><span data-stu-id="9c876-114">Method</span></span>           | <span data-ttu-id="9c876-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9c876-115">Return Type</span></span>    |<span data-ttu-id="9c876-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c876-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c876-117">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="9c876-117">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="9c876-118">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="9c876-118">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="9c876-119">Ler propriedades e relações de um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="9c876-119">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="9c876-120">Update</span><span class="sxs-lookup"><span data-stu-id="9c876-120">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="9c876-121">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="9c876-121">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="9c876-122">Atualize um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="9c876-122">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="9c876-123">Delete</span><span class="sxs-lookup"><span data-stu-id="9c876-123">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="9c876-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c876-124">None</span></span> |<span data-ttu-id="9c876-125">Excluir um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="9c876-125">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c876-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c876-126">Properties</span></span>
| <span data-ttu-id="9c876-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c876-127">Property</span></span>     | <span data-ttu-id="9c876-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c876-128">Type</span></span>   |<span data-ttu-id="9c876-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c876-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c876-130">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="9c876-130">distributeForStudentWork</span></span>|<span data-ttu-id="9c876-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c876-131">Boolean</span></span>|<span data-ttu-id="9c876-132">Indica se esse recurso deve ser copiado para cada aluno enviado para modificação e envio.</span><span class="sxs-lookup"><span data-stu-id="9c876-132">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="9c876-133">id</span><span class="sxs-lookup"><span data-stu-id="9c876-133">id</span></span>|<span data-ttu-id="9c876-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c876-134">String</span></span>| <span data-ttu-id="9c876-135">ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="9c876-135">ID of this resource.</span></span> <span data-ttu-id="9c876-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c876-136">Read-only.</span></span>|
|<span data-ttu-id="9c876-137">recurso</span><span class="sxs-lookup"><span data-stu-id="9c876-137">resource</span></span>|[<span data-ttu-id="9c876-138">educationResource</span><span class="sxs-lookup"><span data-stu-id="9c876-138">educationResource</span></span>](educationresource.md)|<span data-ttu-id="9c876-139">Objeto de recurso que foi associado a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="9c876-139">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c876-140">Relações</span><span class="sxs-lookup"><span data-stu-id="9c876-140">Relationships</span></span>
<span data-ttu-id="9c876-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c876-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9c876-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c876-142">JSON representation</span></span>

<span data-ttu-id="9c876-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c876-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


