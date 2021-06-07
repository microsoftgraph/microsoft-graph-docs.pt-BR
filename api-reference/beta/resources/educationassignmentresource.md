---
title: Tipo de recurso educationAssignmentResource
description: Um objeto wrapper que armazena os recursos associados a uma atribuição. O wrapper adiciona a **propriedade distributeForStudentWork** e indica que esse recurso irá
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a4f4e96c4b08eed4584d6357a8c903c080b2d16d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750366"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="f4ba1-104">Tipo de recurso educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="f4ba1-104">educationAssignmentResource resource type</span></span>

<span data-ttu-id="f4ba1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4ba1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4ba1-106">Um objeto wrapper que armazena os recursos associados a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-106">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="f4ba1-107">O wrapper adiciona **a propriedade distributeForStudentWork** e indica que esse recurso será copiado para o envio do aluno.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-107">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="f4ba1-108">Se o objeto não for copiado, cada aluno verá um link para o recurso na atribuição.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-108">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="f4ba1-109">O aluno não poderá atualizar esse recurso.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-109">The student will not be able to update this resource.</span></span> <span data-ttu-id="f4ba1-110">Esta é uma apostila do professor para o aluno sem nada para ser entregue.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-110">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="f4ba1-111">Se o recurso for distribuído, cada aluno receberá uma cópia desse recurso na lista de recursos de seu envio.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-111">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="f4ba1-112">Cada aluno poderá modificar sua cópia e enviar para a classificação.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-112">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="f4ba1-113">Methods</span><span class="sxs-lookup"><span data-stu-id="f4ba1-113">Methods</span></span>

| <span data-ttu-id="f4ba1-114">Método</span><span class="sxs-lookup"><span data-stu-id="f4ba1-114">Method</span></span>           | <span data-ttu-id="f4ba1-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4ba1-115">Return Type</span></span>    |<span data-ttu-id="f4ba1-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ba1-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4ba1-117">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="f4ba1-117">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="f4ba1-118">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="f4ba1-118">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="f4ba1-119">Leia propriedades e relações de um **objeto educationAssignmentResource.**</span><span class="sxs-lookup"><span data-stu-id="f4ba1-119">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="f4ba1-120">Delete</span><span class="sxs-lookup"><span data-stu-id="f4ba1-120">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="f4ba1-121">None</span><span class="sxs-lookup"><span data-stu-id="f4ba1-121">None</span></span> |<span data-ttu-id="f4ba1-122">**Exclua um objeto educationAssignmentResource.**</span><span class="sxs-lookup"><span data-stu-id="f4ba1-122">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f4ba1-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4ba1-123">Properties</span></span>
| <span data-ttu-id="f4ba1-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4ba1-124">Property</span></span>     | <span data-ttu-id="f4ba1-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ba1-125">Type</span></span>   |<span data-ttu-id="f4ba1-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ba1-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4ba1-127">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="f4ba1-127">distributeForStudentWork</span></span>|<span data-ttu-id="f4ba1-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4ba1-128">Boolean</span></span>|<span data-ttu-id="f4ba1-129">Indica se esse recurso deve ser copiado para cada envio de alunos para modificação e envio.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-129">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="f4ba1-130">id</span><span class="sxs-lookup"><span data-stu-id="f4ba1-130">id</span></span>|<span data-ttu-id="f4ba1-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4ba1-131">String</span></span>| <span data-ttu-id="f4ba1-132">ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-132">ID of this resource.</span></span> <span data-ttu-id="f4ba1-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-133">Read-only.</span></span>|
|<span data-ttu-id="f4ba1-134">recurso</span><span class="sxs-lookup"><span data-stu-id="f4ba1-134">resource</span></span>|[<span data-ttu-id="f4ba1-135">educationResource</span><span class="sxs-lookup"><span data-stu-id="f4ba1-135">educationResource</span></span>](educationresource.md)|<span data-ttu-id="f4ba1-136">Objeto Resource que foi associado a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-136">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4ba1-137">Relações</span><span class="sxs-lookup"><span data-stu-id="f4ba1-137">Relationships</span></span>
<span data-ttu-id="f4ba1-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4ba1-138">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f4ba1-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4ba1-139">JSON representation</span></span>

<span data-ttu-id="f4ba1-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4ba1-140">The following is a JSON representation of the resource.</span></span>

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


