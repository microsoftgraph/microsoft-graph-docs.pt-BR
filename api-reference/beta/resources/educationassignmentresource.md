---
title: tipo de recurso educationAssignmentResource
description: Um objeto envoltório que armazena os recursos associados a uma atribuição. O wrapper adiciona a propriedade **distributeForStudentWork** e indica que este recurso irá
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60181a2289b272809cff025abeee83c594ae833e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006427"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="585d9-104">tipo de recurso educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="585d9-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="585d9-105">Um objeto envoltório que armazena os recursos associados a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="585d9-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="585d9-106">O wrapper adiciona a propriedade **distributeForStudentWork** e indica que esse recurso será copiado para o envio do aluno.</span><span class="sxs-lookup"><span data-stu-id="585d9-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="585d9-107">Se o objeto não for copiado, cada aluno verá um link para o recurso na atribuição.</span><span class="sxs-lookup"><span data-stu-id="585d9-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="585d9-108">O aluno não poderá atualizar esse recurso.</span><span class="sxs-lookup"><span data-stu-id="585d9-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="585d9-109">Este é um folheto do professor para o aluno com nada para ser ativado.</span><span class="sxs-lookup"><span data-stu-id="585d9-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="585d9-110">Se o recurso for distribuído, cada aluno receberá uma cópia desse recurso na lista de recursos do envio.</span><span class="sxs-lookup"><span data-stu-id="585d9-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="585d9-111">Cada aluno poderá modificar a cópia e enviá-la para a gradação.</span><span class="sxs-lookup"><span data-stu-id="585d9-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="585d9-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="585d9-112">Methods</span></span>

| <span data-ttu-id="585d9-113">Método</span><span class="sxs-lookup"><span data-stu-id="585d9-113">Method</span></span>           | <span data-ttu-id="585d9-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="585d9-114">Return Type</span></span>    |<span data-ttu-id="585d9-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="585d9-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="585d9-116">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="585d9-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="585d9-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="585d9-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="585d9-118">Ler propriedades e relações de um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="585d9-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="585d9-119">Atualização</span><span class="sxs-lookup"><span data-stu-id="585d9-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="585d9-120">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="585d9-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="585d9-121">Atualize um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="585d9-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="585d9-122">Delete</span><span class="sxs-lookup"><span data-stu-id="585d9-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="585d9-123">None</span><span class="sxs-lookup"><span data-stu-id="585d9-123">None</span></span> |<span data-ttu-id="585d9-124">Excluir um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="585d9-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="585d9-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="585d9-125">Properties</span></span>
| <span data-ttu-id="585d9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="585d9-126">Property</span></span>     | <span data-ttu-id="585d9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="585d9-127">Type</span></span>   |<span data-ttu-id="585d9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="585d9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="585d9-129">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="585d9-129">distributeForStudentWork</span></span>|<span data-ttu-id="585d9-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="585d9-130">Boolean</span></span>|<span data-ttu-id="585d9-131">Indica se esse recurso deve ser copiado para cada aluno enviado para modificação e envio.</span><span class="sxs-lookup"><span data-stu-id="585d9-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="585d9-132">id</span><span class="sxs-lookup"><span data-stu-id="585d9-132">id</span></span>|<span data-ttu-id="585d9-133">String</span><span class="sxs-lookup"><span data-stu-id="585d9-133">String</span></span>| <span data-ttu-id="585d9-134">ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="585d9-134">ID of this resource.</span></span> <span data-ttu-id="585d9-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="585d9-135">Read-only.</span></span>|
|<span data-ttu-id="585d9-136">recurso</span><span class="sxs-lookup"><span data-stu-id="585d9-136">resource</span></span>|[<span data-ttu-id="585d9-137">educationResource</span><span class="sxs-lookup"><span data-stu-id="585d9-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="585d9-138">Objeto de recurso que foi associado a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="585d9-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="585d9-139">Relações</span><span class="sxs-lookup"><span data-stu-id="585d9-139">Relationships</span></span>
<span data-ttu-id="585d9-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="585d9-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="585d9-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="585d9-141">JSON representation</span></span>

<span data-ttu-id="585d9-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="585d9-142">The following is a JSON representation of the resource.</span></span>

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
