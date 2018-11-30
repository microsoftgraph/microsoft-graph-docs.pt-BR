---
title: tipo de recurso de educationAssignmentResource
description: Um objeto wrapper que armazena os recursos associados a uma atribuição. O wrapper adiciona a propriedade **distributeForStudentWork** e indica as datas que este recurso será
ms.openlocfilehash: 6907af5e4408248487b118c390bb2ec209700124
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037222"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="faa81-104">tipo de recurso de educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="faa81-104">educationAssignmentResource resource type</span></span>

> <span data-ttu-id="faa81-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="faa81-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faa81-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="faa81-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="faa81-107">Um objeto wrapper que armazena os recursos associados a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="faa81-107">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="faa81-108">O wrapper adiciona a propriedade **distributeForStudentWork** e indica as datas que este recurso será copiado para o envio de student.</span><span class="sxs-lookup"><span data-stu-id="faa81-108">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="faa81-109">Se o objeto não for copiado, a cada aluno verão um link para o recurso na atribuição.</span><span class="sxs-lookup"><span data-stu-id="faa81-109">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="faa81-110">O aluno não poderão atualizar esse recurso.</span><span class="sxs-lookup"><span data-stu-id="faa81-110">The student will not be able to update this resource.</span></span> <span data-ttu-id="faa81-111">Este é um folheto do professor ao aluno com nada a ser ativado.</span><span class="sxs-lookup"><span data-stu-id="faa81-111">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="faa81-112">Se o recurso é distribuído, cada aluno receberá uma cópia desse recurso na lista de recursos de envio.</span><span class="sxs-lookup"><span data-stu-id="faa81-112">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="faa81-113">Cada aluno poderá modificar suas cópias e enviá-la para a classificação.</span><span class="sxs-lookup"><span data-stu-id="faa81-113">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="faa81-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="faa81-114">Methods</span></span>

| <span data-ttu-id="faa81-115">Método</span><span class="sxs-lookup"><span data-stu-id="faa81-115">Method</span></span>           | <span data-ttu-id="faa81-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="faa81-116">Return Type</span></span>    |<span data-ttu-id="faa81-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="faa81-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="faa81-118">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="faa81-118">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="faa81-119">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="faa81-119">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="faa81-120">Leia as propriedades e os relacionamentos de um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="faa81-120">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="faa81-121">Update</span><span class="sxs-lookup"><span data-stu-id="faa81-121">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="faa81-122">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="faa81-122">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="faa81-123">Atualize um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="faa81-123">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="faa81-124">Delete</span><span class="sxs-lookup"><span data-stu-id="faa81-124">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="faa81-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="faa81-125">None</span></span> |<span data-ttu-id="faa81-126">Exclua um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="faa81-126">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="faa81-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="faa81-127">Properties</span></span>
| <span data-ttu-id="faa81-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faa81-128">Property</span></span>     | <span data-ttu-id="faa81-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="faa81-129">Type</span></span>   |<span data-ttu-id="faa81-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="faa81-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="faa81-131">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="faa81-131">distributeForStudentWork</span></span>|<span data-ttu-id="faa81-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="faa81-132">Boolean</span></span>|<span data-ttu-id="faa81-133">Indica se este recurso deve ser copiado para cada envio estudante para envio e modificação.</span><span class="sxs-lookup"><span data-stu-id="faa81-133">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="faa81-134">id</span><span class="sxs-lookup"><span data-stu-id="faa81-134">id</span></span>|<span data-ttu-id="faa81-135">String</span><span class="sxs-lookup"><span data-stu-id="faa81-135">String</span></span>| <span data-ttu-id="faa81-136">Identificação desse recurso.</span><span class="sxs-lookup"><span data-stu-id="faa81-136">ID of this resource.</span></span> <span data-ttu-id="faa81-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="faa81-137">Read-only.</span></span>|
|<span data-ttu-id="faa81-138">recurso</span><span class="sxs-lookup"><span data-stu-id="faa81-138">resource</span></span>|[<span data-ttu-id="faa81-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="faa81-139">educationResource</span></span>](educationresource.md)|<span data-ttu-id="faa81-140">Objeto de recurso que tiver sido associado essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="faa81-140">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="faa81-141">Relações</span><span class="sxs-lookup"><span data-stu-id="faa81-141">Relationships</span></span>
<span data-ttu-id="faa81-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="faa81-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="faa81-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="faa81-143">JSON representation</span></span>

<span data-ttu-id="faa81-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="faa81-144">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
