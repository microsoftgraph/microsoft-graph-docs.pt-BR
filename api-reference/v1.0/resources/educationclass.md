---
title: Tipo de recurso educationClass
description: 'Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo Microsoft 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 78280017d71fe0cbcaa84ec22905da6848f45f98
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897880"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="bab16-106">Tipo de recurso educationClass</span><span class="sxs-lookup"><span data-stu-id="bab16-106">educationClass resource type</span></span>

<span data-ttu-id="bab16-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bab16-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bab16-108">Representa uma aula em uma escola.</span><span class="sxs-lookup"><span data-stu-id="bab16-108">Represents a class within a school.</span></span> <span data-ttu-id="bab16-109">O recurso **educationClass** corresponde ao grupo Microsoft 365 e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="bab16-109">The **educationClass** resource corresponds to the Microsoft 365 group and shares the same ID.</span></span> <span data-ttu-id="bab16-110">Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados.</span><span class="sxs-lookup"><span data-stu-id="bab16-110">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="bab16-111">Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.</span><span class="sxs-lookup"><span data-stu-id="bab16-111">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="bab16-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="bab16-112">Methods</span></span>

| <span data-ttu-id="bab16-113">Método</span><span class="sxs-lookup"><span data-stu-id="bab16-113">Method</span></span>           | <span data-ttu-id="bab16-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bab16-114">Return Type</span></span>    |<span data-ttu-id="bab16-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="bab16-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bab16-116">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="bab16-116">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="bab16-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="bab16-117">educationClass</span></span>](educationclass.md) |<span data-ttu-id="bab16-118">Leia as propriedades e relações de um objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="bab16-118">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="bab16-119">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="bab16-119">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="bab16-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="bab16-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="bab16-121">Adicione um novo **educationUser** para a aula postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="bab16-121">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="bab16-122">Listar membros</span><span class="sxs-lookup"><span data-stu-id="bab16-122">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="bab16-123">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="bab16-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="bab16-124">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="bab16-124">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="bab16-125">Remover alunos</span><span class="sxs-lookup"><span data-stu-id="bab16-125">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="bab16-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="bab16-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="bab16-127">Remova um **educationUser** da aula por meio da propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="bab16-127">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="bab16-128">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="bab16-128">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="bab16-129">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="bab16-129">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="bab16-130">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="bab16-130">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="bab16-131">Adicionar professor</span><span class="sxs-lookup"><span data-stu-id="bab16-131">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="bab16-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="bab16-132">educationUser</span></span>](educationuser.md)| <span data-ttu-id="bab16-133">Adicione um novo **educationUser** para a aula postando na propriedade de navegação de professores.</span><span class="sxs-lookup"><span data-stu-id="bab16-133">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="bab16-134">Listar professores</span><span class="sxs-lookup"><span data-stu-id="bab16-134">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="bab16-135">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="bab16-135">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="bab16-136">Obtenha uma lista de professores para a aula.</span><span class="sxs-lookup"><span data-stu-id="bab16-136">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="bab16-137">Remover professor</span><span class="sxs-lookup"><span data-stu-id="bab16-137">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="bab16-138">educationUser</span><span class="sxs-lookup"><span data-stu-id="bab16-138">educationUser</span></span>](educationuser.md)| <span data-ttu-id="bab16-139">Remova um **educationUser** da aula por meio da propriedade de navegação de professores.</span><span class="sxs-lookup"><span data-stu-id="bab16-139">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="bab16-140">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="bab16-140">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="bab16-141">group</span><span class="sxs-lookup"><span data-stu-id="bab16-141">group</span></span>](group.md)| <span data-ttu-id="bab16-142">Obtenha o **grupo** Microsoft 365 que corresponde a esse **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="bab16-142">Get the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="bab16-143">Atualizar</span><span class="sxs-lookup"><span data-stu-id="bab16-143">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="bab16-144">educationClass</span><span class="sxs-lookup"><span data-stu-id="bab16-144">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="bab16-145">Atualize o objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="bab16-145">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="bab16-146">Delete</span><span class="sxs-lookup"><span data-stu-id="bab16-146">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="bab16-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bab16-147">None</span></span> |<span data-ttu-id="bab16-148">Exclua o objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="bab16-148">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bab16-149">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bab16-149">Properties</span></span>
| <span data-ttu-id="bab16-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bab16-150">Property</span></span>     | <span data-ttu-id="bab16-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="bab16-151">Type</span></span>   |<span data-ttu-id="bab16-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="bab16-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bab16-153">id</span><span class="sxs-lookup"><span data-stu-id="bab16-153">id</span></span>| <span data-ttu-id="bab16-154">String</span><span class="sxs-lookup"><span data-stu-id="bab16-154">String</span></span>| <span data-ttu-id="bab16-155">O identificador exclusivo da aula.</span><span class="sxs-lookup"><span data-stu-id="bab16-155">Unique identifier for the class.</span></span>|
|<span data-ttu-id="bab16-156">description</span><span class="sxs-lookup"><span data-stu-id="bab16-156">description</span></span>|<span data-ttu-id="bab16-157">String</span><span class="sxs-lookup"><span data-stu-id="bab16-157">String</span></span>| <span data-ttu-id="bab16-158">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="bab16-158">Description of the class.</span></span>|
|<span data-ttu-id="bab16-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bab16-159">displayName</span></span>|<span data-ttu-id="bab16-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bab16-160">String</span></span>| <span data-ttu-id="bab16-161">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="bab16-161">Name of the class.</span></span>|
|<span data-ttu-id="bab16-162">mailNickname</span><span class="sxs-lookup"><span data-stu-id="bab16-162">mailNickname</span></span>|<span data-ttu-id="bab16-163">String</span><span class="sxs-lookup"><span data-stu-id="bab16-163">String</span></span>| <span data-ttu-id="bab16-164">Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="bab16-164">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="bab16-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="bab16-165">createdBy</span></span>|[<span data-ttu-id="bab16-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="bab16-166">identitySet</span></span>](identityset.md)| <span data-ttu-id="bab16-167">Entidade que criou a aula</span><span class="sxs-lookup"><span data-stu-id="bab16-167">Entity who created the class</span></span> |
|<span data-ttu-id="bab16-168">classCode</span><span class="sxs-lookup"><span data-stu-id="bab16-168">classCode</span></span>|<span data-ttu-id="bab16-169">String</span><span class="sxs-lookup"><span data-stu-id="bab16-169">String</span></span>| <span data-ttu-id="bab16-170">Código de aula usada pela escola para identificar a aula.</span><span class="sxs-lookup"><span data-stu-id="bab16-170">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="bab16-171">externalId</span><span class="sxs-lookup"><span data-stu-id="bab16-171">externalId</span></span>|<span data-ttu-id="bab16-172">String</span><span class="sxs-lookup"><span data-stu-id="bab16-172">String</span></span>| <span data-ttu-id="bab16-173">ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="bab16-173">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="bab16-174">externalName</span><span class="sxs-lookup"><span data-stu-id="bab16-174">externalName</span></span>|<span data-ttu-id="bab16-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bab16-175">String</span></span>|<span data-ttu-id="bab16-176">Nome da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="bab16-176">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="bab16-177">externalSource</span><span class="sxs-lookup"><span data-stu-id="bab16-177">externalSource</span></span>|<span data-ttu-id="bab16-178">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="bab16-178">educationExternalSource</span></span>| <span data-ttu-id="bab16-179">Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="bab16-179">How this class was created.</span></span> <span data-ttu-id="bab16-180">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bab16-180">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bab16-181">term</span><span class="sxs-lookup"><span data-stu-id="bab16-181">term</span></span>|[<span data-ttu-id="bab16-182">educationTerm</span><span class="sxs-lookup"><span data-stu-id="bab16-182">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="bab16-183">Termos dessa aula.</span><span class="sxs-lookup"><span data-stu-id="bab16-183">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bab16-184">Relações</span><span class="sxs-lookup"><span data-stu-id="bab16-184">Relationships</span></span>
| <span data-ttu-id="bab16-185">Relação</span><span class="sxs-lookup"><span data-stu-id="bab16-185">Relationship</span></span> | <span data-ttu-id="bab16-186">Tipo</span><span class="sxs-lookup"><span data-stu-id="bab16-186">Type</span></span>   |<span data-ttu-id="bab16-187">Descrição</span><span class="sxs-lookup"><span data-stu-id="bab16-187">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bab16-188">membros</span><span class="sxs-lookup"><span data-stu-id="bab16-188">members</span></span>|<span data-ttu-id="bab16-189">Coleção [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="bab16-189">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="bab16-190">Todos os usuários da aula.</span><span class="sxs-lookup"><span data-stu-id="bab16-190">All users in the class.</span></span> <span data-ttu-id="bab16-191">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bab16-191">Nullable.</span></span>|
|<span data-ttu-id="bab16-192">schools</span><span class="sxs-lookup"><span data-stu-id="bab16-192">schools</span></span>|<span data-ttu-id="bab16-193">Coleção [educationSchool](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="bab16-193">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="bab16-194">Todas as escolas às quais essa aula está associada.</span><span class="sxs-lookup"><span data-stu-id="bab16-194">All schools that this class is associated with.</span></span> <span data-ttu-id="bab16-195">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bab16-195">Nullable.</span></span>|
|<span data-ttu-id="bab16-196">teachers</span><span class="sxs-lookup"><span data-stu-id="bab16-196">teachers</span></span>|<span data-ttu-id="bab16-197">Coleção [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="bab16-197">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="bab16-198">Todos os professores da aula.</span><span class="sxs-lookup"><span data-stu-id="bab16-198">All teachers in the class.</span></span> <span data-ttu-id="bab16-199">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bab16-199">Nullable.</span></span>|
|<span data-ttu-id="bab16-200">group</span><span class="sxs-lookup"><span data-stu-id="bab16-200">group</span></span>|[<span data-ttu-id="bab16-201">group</span><span class="sxs-lookup"><span data-stu-id="bab16-201">group</span></span>](../resources/group.md)| <span data-ttu-id="bab16-202">O grupo de diretórios correspondente a esta classe.</span><span class="sxs-lookup"><span data-stu-id="bab16-202">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bab16-203">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bab16-203">JSON representation</span></span>

<span data-ttu-id="bab16-204">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bab16-204">The following is a JSON representation of the resource.</span></span>

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
