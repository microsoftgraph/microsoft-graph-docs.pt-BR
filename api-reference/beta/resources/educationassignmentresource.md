---
title: tipo de recurso educationAssignmentResource
description: Um objeto envoltório que armazena os recursos associados a uma atribuição. O wrapper adiciona a propriedade **distributeForStudentWork** e indica que este recurso irá
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 4d05cf5307e77dc6a7ac438c1bd4f4af4e73784e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542934"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="37583-104">tipo de recurso educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="37583-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37583-105">Um objeto envoltório que armazena os recursos associados a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="37583-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="37583-106">O wrapper adiciona a propriedade **distributeForStudentWork** e indica que esse recurso será copiado para o envio do aluno.</span><span class="sxs-lookup"><span data-stu-id="37583-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="37583-107">Se o objeto não for copiado, cada aluno verá um link para o recurso na atribuição.</span><span class="sxs-lookup"><span data-stu-id="37583-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="37583-108">O aluno não poderá atualizar esse recurso.</span><span class="sxs-lookup"><span data-stu-id="37583-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="37583-109">Este é um folheto do professor para o aluno com nada para ser ativado.</span><span class="sxs-lookup"><span data-stu-id="37583-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="37583-110">Se o recurso for distribuído, cada aluno receberá uma cópia desse recurso na lista de recursos do envio.</span><span class="sxs-lookup"><span data-stu-id="37583-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="37583-111">Cada aluno poderá modificar a cópia e enviá-la para a gradação.</span><span class="sxs-lookup"><span data-stu-id="37583-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="37583-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="37583-112">Methods</span></span>

| <span data-ttu-id="37583-113">Método</span><span class="sxs-lookup"><span data-stu-id="37583-113">Method</span></span>           | <span data-ttu-id="37583-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="37583-114">Return Type</span></span>    |<span data-ttu-id="37583-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="37583-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37583-116">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="37583-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="37583-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="37583-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="37583-118">Ler propriedades e relações de um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="37583-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="37583-119">Update</span><span class="sxs-lookup"><span data-stu-id="37583-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="37583-120">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="37583-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="37583-121">Atualize um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="37583-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="37583-122">Excluir</span><span class="sxs-lookup"><span data-stu-id="37583-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="37583-123">None</span><span class="sxs-lookup"><span data-stu-id="37583-123">None</span></span> |<span data-ttu-id="37583-124">Excluir um objeto **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="37583-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="37583-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37583-125">Properties</span></span>
| <span data-ttu-id="37583-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37583-126">Property</span></span>     | <span data-ttu-id="37583-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="37583-127">Type</span></span>   |<span data-ttu-id="37583-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="37583-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37583-129">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="37583-129">distributeForStudentWork</span></span>|<span data-ttu-id="37583-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="37583-130">Boolean</span></span>|<span data-ttu-id="37583-131">Indica se esse recurso deve ser copiado para cada aluno enviado para modificação e envio.</span><span class="sxs-lookup"><span data-stu-id="37583-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="37583-132">id</span><span class="sxs-lookup"><span data-stu-id="37583-132">id</span></span>|<span data-ttu-id="37583-133">String</span><span class="sxs-lookup"><span data-stu-id="37583-133">String</span></span>| <span data-ttu-id="37583-134">ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="37583-134">ID of this resource.</span></span> <span data-ttu-id="37583-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37583-135">Read-only.</span></span>|
|<span data-ttu-id="37583-136">recurso</span><span class="sxs-lookup"><span data-stu-id="37583-136">resource</span></span>|[<span data-ttu-id="37583-137">educationResource</span><span class="sxs-lookup"><span data-stu-id="37583-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="37583-138">Objeto de recurso que foi associado a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="37583-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37583-139">Relações</span><span class="sxs-lookup"><span data-stu-id="37583-139">Relationships</span></span>
<span data-ttu-id="37583-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37583-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="37583-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37583-141">JSON representation</span></span>

<span data-ttu-id="37583-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37583-142">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
