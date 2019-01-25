---
title: Tipo de recurso educationClass
description: 'Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5a4bbc0560f2a40b5a438ec8276bbcf984a22721
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526729"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="60586-106">Tipo de recurso educationClass</span><span class="sxs-lookup"><span data-stu-id="60586-106">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60586-107">Representa uma aula em uma escola.</span><span class="sxs-lookup"><span data-stu-id="60586-107">Represents a class within a school.</span></span> <span data-ttu-id="60586-108">O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="60586-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="60586-109">Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados.</span><span class="sxs-lookup"><span data-stu-id="60586-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="60586-110">Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.</span><span class="sxs-lookup"><span data-stu-id="60586-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="60586-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="60586-111">Methods</span></span>

| <span data-ttu-id="60586-112">Método</span><span class="sxs-lookup"><span data-stu-id="60586-112">Method</span></span>           | <span data-ttu-id="60586-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="60586-113">Return Type</span></span>    |<span data-ttu-id="60586-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="60586-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60586-115">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="60586-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="60586-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="60586-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="60586-117">Leia as propriedades e relações de um objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="60586-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="60586-118">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="60586-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="60586-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="60586-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="60586-120">Adicione um novo **educationUser** para a aula postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="60586-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="60586-121">Listar membros</span><span class="sxs-lookup"><span data-stu-id="60586-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="60586-122">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="60586-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="60586-123">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="60586-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="60586-124">Remover alunos</span><span class="sxs-lookup"><span data-stu-id="60586-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="60586-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="60586-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="60586-126">Remova um **educationUser** da aula por meio da propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="60586-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="60586-127">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="60586-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="60586-128">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="60586-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="60586-129">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="60586-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="60586-130">Adicionar professor</span><span class="sxs-lookup"><span data-stu-id="60586-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="60586-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="60586-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="60586-132">Adicione um novo **educationUser** para a aula postando na propriedade de navegação de professores.</span><span class="sxs-lookup"><span data-stu-id="60586-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="60586-133">Listar professores</span><span class="sxs-lookup"><span data-stu-id="60586-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="60586-134">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="60586-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="60586-135">Obtenha uma lista de professores para a aula.</span><span class="sxs-lookup"><span data-stu-id="60586-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="60586-136">Remover professor</span><span class="sxs-lookup"><span data-stu-id="60586-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="60586-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="60586-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="60586-138">Remova um **educationUser** da aula por meio da propriedade de navegação de professores.</span><span class="sxs-lookup"><span data-stu-id="60586-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="60586-139">Criar educationAssignment</span><span class="sxs-lookup"><span data-stu-id="60586-139">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="60586-140">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="60586-140">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="60586-141">Crie um novo **educationAssignment** pelo lançamento para a coleção assignments.</span><span class="sxs-lookup"><span data-stu-id="60586-141">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="60586-142">Lista de atribuições</span><span class="sxs-lookup"><span data-stu-id="60586-142">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="60586-143">coleção [educationAssignment](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="60586-143">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="60586-144">Obtenha uma coleção de objetos **educationAssignment** .</span><span class="sxs-lookup"><span data-stu-id="60586-144">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="60586-145">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="60586-145">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="60586-146">group</span><span class="sxs-lookup"><span data-stu-id="60586-146">group</span></span>](group.md)| <span data-ttu-id="60586-147">Recupere o **group** do Office 365 que corresponde a essa **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="60586-147">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="60586-148">Atualizar</span><span class="sxs-lookup"><span data-stu-id="60586-148">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="60586-149">educationClass</span><span class="sxs-lookup"><span data-stu-id="60586-149">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="60586-150">Atualize o objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="60586-150">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="60586-151">Excluir</span><span class="sxs-lookup"><span data-stu-id="60586-151">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="60586-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60586-152">None</span></span> |<span data-ttu-id="60586-153">Exclua o objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="60586-153">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="60586-154">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60586-154">Properties</span></span>
| <span data-ttu-id="60586-155">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60586-155">Property</span></span>     | <span data-ttu-id="60586-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="60586-156">Type</span></span>   |<span data-ttu-id="60586-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="60586-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60586-158">id</span><span class="sxs-lookup"><span data-stu-id="60586-158">id</span></span>| <span data-ttu-id="60586-159">String</span><span class="sxs-lookup"><span data-stu-id="60586-159">String</span></span>| <span data-ttu-id="60586-160">O identificador exclusivo da aula.</span><span class="sxs-lookup"><span data-stu-id="60586-160">Unique identifier for the class.</span></span>|
|<span data-ttu-id="60586-161">description</span><span class="sxs-lookup"><span data-stu-id="60586-161">description</span></span>|<span data-ttu-id="60586-162">String</span><span class="sxs-lookup"><span data-stu-id="60586-162">String</span></span>| <span data-ttu-id="60586-163">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="60586-163">Description of the class.</span></span>|
|<span data-ttu-id="60586-164">displayName</span><span class="sxs-lookup"><span data-stu-id="60586-164">displayName</span></span>|<span data-ttu-id="60586-165">String</span><span class="sxs-lookup"><span data-stu-id="60586-165">String</span></span>| <span data-ttu-id="60586-166">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="60586-166">Name of the class.</span></span>|
|<span data-ttu-id="60586-167">mailNickname</span><span class="sxs-lookup"><span data-stu-id="60586-167">mailNickname</span></span>|<span data-ttu-id="60586-168">String</span><span class="sxs-lookup"><span data-stu-id="60586-168">String</span></span>| <span data-ttu-id="60586-169">Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="60586-169">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="60586-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="60586-170">createdBy</span></span>|[<span data-ttu-id="60586-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="60586-171">identitySet</span></span>](identityset.md)| <span data-ttu-id="60586-172">Entidade que criou a aula</span><span class="sxs-lookup"><span data-stu-id="60586-172">Entity who created the class</span></span> |
|<span data-ttu-id="60586-173">classCode</span><span class="sxs-lookup"><span data-stu-id="60586-173">classCode</span></span>|<span data-ttu-id="60586-174">String</span><span class="sxs-lookup"><span data-stu-id="60586-174">String</span></span>| <span data-ttu-id="60586-175">Código de aula usada pela escola para identificar a aula.</span><span class="sxs-lookup"><span data-stu-id="60586-175">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="60586-176">externalId</span><span class="sxs-lookup"><span data-stu-id="60586-176">externalId</span></span>|<span data-ttu-id="60586-177">String</span><span class="sxs-lookup"><span data-stu-id="60586-177">String</span></span>| <span data-ttu-id="60586-178">ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="60586-178">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="60586-179">externalName</span><span class="sxs-lookup"><span data-stu-id="60586-179">externalName</span></span>|<span data-ttu-id="60586-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60586-180">String</span></span>|<span data-ttu-id="60586-181">Nome da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="60586-181">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="60586-182">externalSource</span><span class="sxs-lookup"><span data-stu-id="60586-182">externalSource</span></span>|<span data-ttu-id="60586-183">string</span><span class="sxs-lookup"><span data-stu-id="60586-183">string</span></span>| <span data-ttu-id="60586-184">Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="60586-184">How this class was created.</span></span> <span data-ttu-id="60586-185">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="60586-185">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="60586-186">term</span><span class="sxs-lookup"><span data-stu-id="60586-186">term</span></span>|[<span data-ttu-id="60586-187">educationTerm</span><span class="sxs-lookup"><span data-stu-id="60586-187">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="60586-188">Termos dessa aula.</span><span class="sxs-lookup"><span data-stu-id="60586-188">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="60586-189">Relações</span><span class="sxs-lookup"><span data-stu-id="60586-189">Relationships</span></span>
| <span data-ttu-id="60586-190">Relação</span><span class="sxs-lookup"><span data-stu-id="60586-190">Relationship</span></span> | <span data-ttu-id="60586-191">Tipo</span><span class="sxs-lookup"><span data-stu-id="60586-191">Type</span></span>   |<span data-ttu-id="60586-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="60586-192">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60586-193">members</span><span class="sxs-lookup"><span data-stu-id="60586-193">members</span></span>|<span data-ttu-id="60586-194">Coleção [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="60586-194">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="60586-195">Todos os usuários da aula.</span><span class="sxs-lookup"><span data-stu-id="60586-195">All users in the class.</span></span> <span data-ttu-id="60586-196">Anulável.</span><span class="sxs-lookup"><span data-stu-id="60586-196">Nullable.</span></span>|
|<span data-ttu-id="60586-197">schools</span><span class="sxs-lookup"><span data-stu-id="60586-197">schools</span></span>|<span data-ttu-id="60586-198">Coleção [educationSchool](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="60586-198">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="60586-199">Todas as escolas às quais essa aula está associada.</span><span class="sxs-lookup"><span data-stu-id="60586-199">All schools that this class is associated with.</span></span> <span data-ttu-id="60586-200">Anulável.</span><span class="sxs-lookup"><span data-stu-id="60586-200">Nullable.</span></span>|
|<span data-ttu-id="60586-201">teachers</span><span class="sxs-lookup"><span data-stu-id="60586-201">teachers</span></span>|<span data-ttu-id="60586-202">Coleção [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="60586-202">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="60586-203">Todos os professores da aula.</span><span class="sxs-lookup"><span data-stu-id="60586-203">All teachers in the class.</span></span> <span data-ttu-id="60586-204">Anulável.</span><span class="sxs-lookup"><span data-stu-id="60586-204">Nullable.</span></span>|
|<span data-ttu-id="60586-205">assignments</span><span class="sxs-lookup"><span data-stu-id="60586-205">assignments</span></span>|<span data-ttu-id="60586-206">coleção [educationAssignment](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="60586-206">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="60586-207">Todas as atribuições associadas a esta classe.</span><span class="sxs-lookup"><span data-stu-id="60586-207">All assignments associated with this class.</span></span> <span data-ttu-id="60586-208">Anulável.</span><span class="sxs-lookup"><span data-stu-id="60586-208">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60586-209">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60586-209">JSON representation</span></span>

<span data-ttu-id="60586-210">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60586-210">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationclass.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
