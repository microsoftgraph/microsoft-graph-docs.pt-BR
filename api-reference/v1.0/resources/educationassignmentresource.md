---
title: Tipo de recurso educationAssignmentResource
description: Um objeto wrapper que armazena os recursos associados a uma atribuição.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d301eb8f0d9b9f13197be01b2bcf3ccf4297fa24
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912199"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="db79f-103">Tipo de recurso educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="db79f-103">educationAssignmentResource resource type</span></span>

<span data-ttu-id="db79f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db79f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db79f-105">Um objeto wrapper que armazena os recursos associados a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="db79f-105">A wrapper object that stores the resources associated with an assignment.</span></span> 

<span data-ttu-id="db79f-106">O wrapper adiciona **a propriedade distributeForStudentWork** e indica que esse recurso será copiado para o envio do aluno.</span><span class="sxs-lookup"><span data-stu-id="db79f-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="db79f-107">Se o objeto não for copiado, cada aluno verá um link para o recurso na atribuição.</span><span class="sxs-lookup"><span data-stu-id="db79f-107">If the object isn't copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="db79f-108">O aluno não poderá atualizar esse recurso.</span><span class="sxs-lookup"><span data-stu-id="db79f-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="db79f-109">Esta é uma apostila do professor para o aluno sem nada para ser entregue.</span><span class="sxs-lookup"><span data-stu-id="db79f-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="db79f-110">Se o recurso for distribuído, cada aluno receberá uma cópia desse recurso na lista de recursos de seu envio.</span><span class="sxs-lookup"><span data-stu-id="db79f-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="db79f-111">Cada aluno poderá modificar sua cópia e enviar para a classificação.</span><span class="sxs-lookup"><span data-stu-id="db79f-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="db79f-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="db79f-112">Methods</span></span>

| <span data-ttu-id="db79f-113">Método</span><span class="sxs-lookup"><span data-stu-id="db79f-113">Method</span></span>           | <span data-ttu-id="db79f-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="db79f-114">Return Type</span></span>    |<span data-ttu-id="db79f-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="db79f-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db79f-116">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="db79f-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="db79f-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="db79f-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="db79f-118">Leia propriedades e relações de um **objeto educationAssignmentResource.**</span><span class="sxs-lookup"><span data-stu-id="db79f-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="db79f-119">Delete</span><span class="sxs-lookup"><span data-stu-id="db79f-119">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="db79f-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db79f-120">None</span></span> |<span data-ttu-id="db79f-121">**Exclua um objeto educationAssignmentResource.**</span><span class="sxs-lookup"><span data-stu-id="db79f-121">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="db79f-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db79f-122">Properties</span></span>
| <span data-ttu-id="db79f-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db79f-123">Property</span></span>     | <span data-ttu-id="db79f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="db79f-124">Type</span></span>   |<span data-ttu-id="db79f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="db79f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db79f-126">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="db79f-126">distributeForStudentWork</span></span>|<span data-ttu-id="db79f-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="db79f-127">Boolean</span></span>|<span data-ttu-id="db79f-128">Indica se esse recurso deve ser copiado para cada envio de alunos para modificação e envio.</span><span class="sxs-lookup"><span data-stu-id="db79f-128">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="db79f-129">id</span><span class="sxs-lookup"><span data-stu-id="db79f-129">id</span></span>|<span data-ttu-id="db79f-130">String</span><span class="sxs-lookup"><span data-stu-id="db79f-130">String</span></span>| <span data-ttu-id="db79f-131">ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="db79f-131">ID of this resource.</span></span> <span data-ttu-id="db79f-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db79f-132">Read-only.</span></span>|
|<span data-ttu-id="db79f-133">recurso</span><span class="sxs-lookup"><span data-stu-id="db79f-133">resource</span></span>|[<span data-ttu-id="db79f-134">educationResource</span><span class="sxs-lookup"><span data-stu-id="db79f-134">educationResource</span></span>](educationresource.md)|<span data-ttu-id="db79f-135">Objeto Resource que foi associado a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="db79f-135">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db79f-136">Relações</span><span class="sxs-lookup"><span data-stu-id="db79f-136">Relationships</span></span>
<span data-ttu-id="db79f-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db79f-137">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="db79f-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db79f-138">JSON representation</span></span>

<span data-ttu-id="db79f-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db79f-139">The following is a JSON representation of the resource.</span></span>

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


