---
title: Tipo de recurso educationClass
description: 'Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: c5b145d12dd99293eef9c338ff840d5781c5ef3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933985"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="d4792-106">Tipo de recurso educationClass</span><span class="sxs-lookup"><span data-stu-id="d4792-106">educationClass resource type</span></span>

<span data-ttu-id="d4792-107">Representa uma aula em uma escola.</span><span class="sxs-lookup"><span data-stu-id="d4792-107">Represents a class within a school.</span></span> <span data-ttu-id="d4792-108">O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="d4792-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="d4792-109">Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados.</span><span class="sxs-lookup"><span data-stu-id="d4792-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="d4792-110">Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.</span><span class="sxs-lookup"><span data-stu-id="d4792-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="d4792-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="d4792-111">Methods</span></span>

| <span data-ttu-id="d4792-112">Método</span><span class="sxs-lookup"><span data-stu-id="d4792-112">Method</span></span>           | <span data-ttu-id="d4792-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4792-113">Return Type</span></span>    |<span data-ttu-id="d4792-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4792-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4792-115">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="d4792-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="d4792-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="d4792-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="d4792-117">Leia as propriedades e relações de um objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="d4792-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="d4792-118">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="d4792-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="d4792-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="d4792-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="d4792-120">Adicione um novo **educationUser** para a aula postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="d4792-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="d4792-121">Listar membros</span><span class="sxs-lookup"><span data-stu-id="d4792-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="d4792-122">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="d4792-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="d4792-123">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="d4792-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="d4792-124">Remover alunos</span><span class="sxs-lookup"><span data-stu-id="d4792-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="d4792-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="d4792-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="d4792-126">Remova um **educationUser** da aula por meio da propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="d4792-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="d4792-127">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="d4792-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="d4792-128">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="d4792-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="d4792-129">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="d4792-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="d4792-130">Adicionar professor</span><span class="sxs-lookup"><span data-stu-id="d4792-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="d4792-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="d4792-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="d4792-132">Adicione um novo **educationUser** para a aula postando na propriedade de navegação de professores.</span><span class="sxs-lookup"><span data-stu-id="d4792-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="d4792-133">Listar professores</span><span class="sxs-lookup"><span data-stu-id="d4792-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="d4792-134">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="d4792-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="d4792-135">Obtenha uma lista de professores para a aula.</span><span class="sxs-lookup"><span data-stu-id="d4792-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="d4792-136">Remover professor</span><span class="sxs-lookup"><span data-stu-id="d4792-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="d4792-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="d4792-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="d4792-138">Remova um **educationUser** da aula por meio da propriedade de navegação de professores.</span><span class="sxs-lookup"><span data-stu-id="d4792-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="d4792-139">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="d4792-139">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="d4792-140">group</span><span class="sxs-lookup"><span data-stu-id="d4792-140">group</span></span>](group.md)| <span data-ttu-id="d4792-141">Recupere o **group** do Office 365 que corresponde a essa **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="d4792-141">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="d4792-142">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d4792-142">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="d4792-143">educationClass</span><span class="sxs-lookup"><span data-stu-id="d4792-143">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="d4792-144">Atualize o objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="d4792-144">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="d4792-145">Excluir</span><span class="sxs-lookup"><span data-stu-id="d4792-145">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="d4792-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4792-146">None</span></span> |<span data-ttu-id="d4792-147">Exclua o objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="d4792-147">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4792-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4792-148">Properties</span></span>
| <span data-ttu-id="d4792-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4792-149">Property</span></span>     | <span data-ttu-id="d4792-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4792-150">Type</span></span>   |<span data-ttu-id="d4792-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4792-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4792-152">id</span><span class="sxs-lookup"><span data-stu-id="d4792-152">id</span></span>| <span data-ttu-id="d4792-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4792-153">String</span></span>| <span data-ttu-id="d4792-154">O identificador exclusivo da aula.</span><span class="sxs-lookup"><span data-stu-id="d4792-154">Unique identifier for the class.</span></span>|
|<span data-ttu-id="d4792-155">description</span><span class="sxs-lookup"><span data-stu-id="d4792-155">description</span></span>|<span data-ttu-id="d4792-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4792-156">String</span></span>| <span data-ttu-id="d4792-157">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="d4792-157">Description of the class.</span></span>|
|<span data-ttu-id="d4792-158">displayName</span><span class="sxs-lookup"><span data-stu-id="d4792-158">displayName</span></span>|<span data-ttu-id="d4792-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4792-159">String</span></span>| <span data-ttu-id="d4792-160">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="d4792-160">Name of the class.</span></span>|
|<span data-ttu-id="d4792-161">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d4792-161">mailNickname</span></span>|<span data-ttu-id="d4792-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4792-162">String</span></span>| <span data-ttu-id="d4792-163">Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="d4792-163">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="d4792-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="d4792-164">createdBy</span></span>|[<span data-ttu-id="d4792-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="d4792-165">identitySet</span></span>](identityset.md)| <span data-ttu-id="d4792-166">Entidade que criou a aula</span><span class="sxs-lookup"><span data-stu-id="d4792-166">Entity who created the class</span></span> |
|<span data-ttu-id="d4792-167">classCode</span><span class="sxs-lookup"><span data-stu-id="d4792-167">classCode</span></span>|<span data-ttu-id="d4792-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4792-168">String</span></span>| <span data-ttu-id="d4792-169">Código de aula usada pela escola para identificar a aula.</span><span class="sxs-lookup"><span data-stu-id="d4792-169">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="d4792-170">externalId</span><span class="sxs-lookup"><span data-stu-id="d4792-170">externalId</span></span>|<span data-ttu-id="d4792-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4792-171">String</span></span>| <span data-ttu-id="d4792-172">ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="d4792-172">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="d4792-173">externalName</span><span class="sxs-lookup"><span data-stu-id="d4792-173">externalName</span></span>|<span data-ttu-id="d4792-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4792-174">String</span></span>|<span data-ttu-id="d4792-175">Nome da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="d4792-175">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="d4792-176">externalSource</span><span class="sxs-lookup"><span data-stu-id="d4792-176">externalSource</span></span>|<span data-ttu-id="d4792-177">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="d4792-177">educationExternalSource</span></span>| <span data-ttu-id="d4792-178">Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="d4792-178">How this class was created.</span></span> <span data-ttu-id="d4792-179">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d4792-179">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d4792-180">term</span><span class="sxs-lookup"><span data-stu-id="d4792-180">term</span></span>|[<span data-ttu-id="d4792-181">educationTerm</span><span class="sxs-lookup"><span data-stu-id="d4792-181">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="d4792-182">Termos dessa aula.</span><span class="sxs-lookup"><span data-stu-id="d4792-182">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4792-183">Relações</span><span class="sxs-lookup"><span data-stu-id="d4792-183">Relationships</span></span>
| <span data-ttu-id="d4792-184">Relação</span><span class="sxs-lookup"><span data-stu-id="d4792-184">Relationship</span></span> | <span data-ttu-id="d4792-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4792-185">Type</span></span>   |<span data-ttu-id="d4792-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4792-186">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4792-187">members</span><span class="sxs-lookup"><span data-stu-id="d4792-187">members</span></span>|<span data-ttu-id="d4792-188">Coleção [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="d4792-188">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="d4792-189">Todos os usuários da aula.</span><span class="sxs-lookup"><span data-stu-id="d4792-189">All users in the class.</span></span> <span data-ttu-id="d4792-190">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d4792-190">Nullable.</span></span>|
|<span data-ttu-id="d4792-191">schools</span><span class="sxs-lookup"><span data-stu-id="d4792-191">schools</span></span>|<span data-ttu-id="d4792-192">Coleção [educationSchool](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="d4792-192">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="d4792-193">Todas as escolas às quais essa aula está associada.</span><span class="sxs-lookup"><span data-stu-id="d4792-193">All schools that this class is associated with.</span></span> <span data-ttu-id="d4792-194">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d4792-194">Nullable.</span></span>|
|<span data-ttu-id="d4792-195">teachers</span><span class="sxs-lookup"><span data-stu-id="d4792-195">teachers</span></span>|<span data-ttu-id="d4792-196">Coleção [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="d4792-196">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="d4792-197">Todos os professores da aula.</span><span class="sxs-lookup"><span data-stu-id="d4792-197">All teachers in the class.</span></span> <span data-ttu-id="d4792-198">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d4792-198">Nullable.</span></span>|
|<span data-ttu-id="d4792-199">group</span><span class="sxs-lookup"><span data-stu-id="d4792-199">group</span></span>|[<span data-ttu-id="d4792-200">grupo</span><span class="sxs-lookup"><span data-stu-id="d4792-200">group</span></span>](../resources/group.md)| <span data-ttu-id="d4792-201">O grupo de diretório correspondente a esta classe.</span><span class="sxs-lookup"><span data-stu-id="d4792-201">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4792-202">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4792-202">JSON representation</span></span>

<span data-ttu-id="d4792-203">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4792-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
