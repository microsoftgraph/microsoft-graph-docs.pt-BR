---
title: Tipo de recurso educationClass
description: 'Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d767f25fd5d383d297f3765498f3558a162f2716
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531535"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="625a0-106">Tipo de recurso educationClass</span><span class="sxs-lookup"><span data-stu-id="625a0-106">educationClass resource type</span></span>

<span data-ttu-id="625a0-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="625a0-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="625a0-108">Representa uma aula em uma escola.</span><span class="sxs-lookup"><span data-stu-id="625a0-108">Represents a class within a school.</span></span> <span data-ttu-id="625a0-109">O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="625a0-109">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="625a0-110">Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados.</span><span class="sxs-lookup"><span data-stu-id="625a0-110">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="625a0-111">Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.</span><span class="sxs-lookup"><span data-stu-id="625a0-111">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="625a0-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="625a0-112">Methods</span></span>

| <span data-ttu-id="625a0-113">Método</span><span class="sxs-lookup"><span data-stu-id="625a0-113">Method</span></span>           | <span data-ttu-id="625a0-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="625a0-114">Return Type</span></span>    |<span data-ttu-id="625a0-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="625a0-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="625a0-116">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="625a0-116">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="625a0-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="625a0-117">educationClass</span></span>](educationclass.md) |<span data-ttu-id="625a0-118">Leia as propriedades e relações de um objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="625a0-118">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="625a0-119">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="625a0-119">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="625a0-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="625a0-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="625a0-121">Adicione um novo **educationUser** para a aula postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="625a0-121">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="625a0-122">Listar membros</span><span class="sxs-lookup"><span data-stu-id="625a0-122">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="625a0-123">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="625a0-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="625a0-124">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="625a0-124">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="625a0-125">Remover alunos</span><span class="sxs-lookup"><span data-stu-id="625a0-125">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="625a0-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="625a0-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="625a0-127">Remova um **educationUser** da aula por meio da propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="625a0-127">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="625a0-128">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="625a0-128">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="625a0-129">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="625a0-129">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="625a0-130">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="625a0-130">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="625a0-131">Adicionar professor</span><span class="sxs-lookup"><span data-stu-id="625a0-131">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="625a0-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="625a0-132">educationUser</span></span>](educationuser.md)| <span data-ttu-id="625a0-133">Adicione um novo **educationUser** para a aula postando na propriedade de navegação de professores.</span><span class="sxs-lookup"><span data-stu-id="625a0-133">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="625a0-134">Listar professores</span><span class="sxs-lookup"><span data-stu-id="625a0-134">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="625a0-135">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="625a0-135">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="625a0-136">Obtenha uma lista de professores para a aula.</span><span class="sxs-lookup"><span data-stu-id="625a0-136">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="625a0-137">Remover professor</span><span class="sxs-lookup"><span data-stu-id="625a0-137">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="625a0-138">educationUser</span><span class="sxs-lookup"><span data-stu-id="625a0-138">educationUser</span></span>](educationuser.md)| <span data-ttu-id="625a0-139">Remova um **educationUser** da aula por meio da propriedade de navegação de professores.</span><span class="sxs-lookup"><span data-stu-id="625a0-139">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="625a0-140">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="625a0-140">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="625a0-141">group</span><span class="sxs-lookup"><span data-stu-id="625a0-141">group</span></span>](group.md)| <span data-ttu-id="625a0-142">Recupere o **group** do Office 365 que corresponde a essa **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="625a0-142">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="625a0-143">Atualizar</span><span class="sxs-lookup"><span data-stu-id="625a0-143">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="625a0-144">educationClass</span><span class="sxs-lookup"><span data-stu-id="625a0-144">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="625a0-145">Atualize o objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="625a0-145">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="625a0-146">Excluir</span><span class="sxs-lookup"><span data-stu-id="625a0-146">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="625a0-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="625a0-147">None</span></span> |<span data-ttu-id="625a0-148">Exclua o objeto **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="625a0-148">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="625a0-149">Propriedades</span><span class="sxs-lookup"><span data-stu-id="625a0-149">Properties</span></span>
| <span data-ttu-id="625a0-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="625a0-150">Property</span></span>     | <span data-ttu-id="625a0-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="625a0-151">Type</span></span>   |<span data-ttu-id="625a0-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="625a0-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="625a0-153">id</span><span class="sxs-lookup"><span data-stu-id="625a0-153">id</span></span>| <span data-ttu-id="625a0-154">String</span><span class="sxs-lookup"><span data-stu-id="625a0-154">String</span></span>| <span data-ttu-id="625a0-155">O identificador exclusivo da aula.</span><span class="sxs-lookup"><span data-stu-id="625a0-155">Unique identifier for the class.</span></span>|
|<span data-ttu-id="625a0-156">description</span><span class="sxs-lookup"><span data-stu-id="625a0-156">description</span></span>|<span data-ttu-id="625a0-157">String</span><span class="sxs-lookup"><span data-stu-id="625a0-157">String</span></span>| <span data-ttu-id="625a0-158">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="625a0-158">Description of the class.</span></span>|
|<span data-ttu-id="625a0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="625a0-159">displayName</span></span>|<span data-ttu-id="625a0-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="625a0-160">String</span></span>| <span data-ttu-id="625a0-161">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="625a0-161">Name of the class.</span></span>|
|<span data-ttu-id="625a0-162">mailNickname</span><span class="sxs-lookup"><span data-stu-id="625a0-162">mailNickname</span></span>|<span data-ttu-id="625a0-163">String</span><span class="sxs-lookup"><span data-stu-id="625a0-163">String</span></span>| <span data-ttu-id="625a0-164">Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="625a0-164">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="625a0-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="625a0-165">createdBy</span></span>|[<span data-ttu-id="625a0-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="625a0-166">identitySet</span></span>](identityset.md)| <span data-ttu-id="625a0-167">Entidade que criou a aula</span><span class="sxs-lookup"><span data-stu-id="625a0-167">Entity who created the class</span></span> |
|<span data-ttu-id="625a0-168">classCode</span><span class="sxs-lookup"><span data-stu-id="625a0-168">classCode</span></span>|<span data-ttu-id="625a0-169">String</span><span class="sxs-lookup"><span data-stu-id="625a0-169">String</span></span>| <span data-ttu-id="625a0-170">Código de aula usada pela escola para identificar a aula.</span><span class="sxs-lookup"><span data-stu-id="625a0-170">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="625a0-171">externalId</span><span class="sxs-lookup"><span data-stu-id="625a0-171">externalId</span></span>|<span data-ttu-id="625a0-172">String</span><span class="sxs-lookup"><span data-stu-id="625a0-172">String</span></span>| <span data-ttu-id="625a0-173">ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="625a0-173">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="625a0-174">externalName</span><span class="sxs-lookup"><span data-stu-id="625a0-174">externalName</span></span>|<span data-ttu-id="625a0-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="625a0-175">String</span></span>|<span data-ttu-id="625a0-176">Nome da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="625a0-176">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="625a0-177">externalSource</span><span class="sxs-lookup"><span data-stu-id="625a0-177">externalSource</span></span>|<span data-ttu-id="625a0-178">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="625a0-178">educationExternalSource</span></span>| <span data-ttu-id="625a0-179">Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="625a0-179">How this class was created.</span></span> <span data-ttu-id="625a0-180">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="625a0-180">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="625a0-181">term</span><span class="sxs-lookup"><span data-stu-id="625a0-181">term</span></span>|[<span data-ttu-id="625a0-182">educationTerm</span><span class="sxs-lookup"><span data-stu-id="625a0-182">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="625a0-183">Termos dessa aula.</span><span class="sxs-lookup"><span data-stu-id="625a0-183">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="625a0-184">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="625a0-184">Relationships</span></span>
| <span data-ttu-id="625a0-185">Relação</span><span class="sxs-lookup"><span data-stu-id="625a0-185">Relationship</span></span> | <span data-ttu-id="625a0-186">Tipo</span><span class="sxs-lookup"><span data-stu-id="625a0-186">Type</span></span>   |<span data-ttu-id="625a0-187">Descrição</span><span class="sxs-lookup"><span data-stu-id="625a0-187">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="625a0-188">membros</span><span class="sxs-lookup"><span data-stu-id="625a0-188">members</span></span>|<span data-ttu-id="625a0-189">Coleção [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="625a0-189">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="625a0-190">Todos os usuários da aula.</span><span class="sxs-lookup"><span data-stu-id="625a0-190">All users in the class.</span></span> <span data-ttu-id="625a0-191">Anulável.</span><span class="sxs-lookup"><span data-stu-id="625a0-191">Nullable.</span></span>|
|<span data-ttu-id="625a0-192">schools</span><span class="sxs-lookup"><span data-stu-id="625a0-192">schools</span></span>|<span data-ttu-id="625a0-193">Coleção [educationSchool](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="625a0-193">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="625a0-194">Todas as escolas às quais essa aula está associada.</span><span class="sxs-lookup"><span data-stu-id="625a0-194">All schools that this class is associated with.</span></span> <span data-ttu-id="625a0-195">Anulável.</span><span class="sxs-lookup"><span data-stu-id="625a0-195">Nullable.</span></span>|
|<span data-ttu-id="625a0-196">teachers</span><span class="sxs-lookup"><span data-stu-id="625a0-196">teachers</span></span>|<span data-ttu-id="625a0-197">Coleção [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="625a0-197">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="625a0-198">Todos os professores da aula.</span><span class="sxs-lookup"><span data-stu-id="625a0-198">All teachers in the class.</span></span> <span data-ttu-id="625a0-199">Anulável.</span><span class="sxs-lookup"><span data-stu-id="625a0-199">Nullable.</span></span>|
|<span data-ttu-id="625a0-200">group</span><span class="sxs-lookup"><span data-stu-id="625a0-200">group</span></span>|[<span data-ttu-id="625a0-201">group</span><span class="sxs-lookup"><span data-stu-id="625a0-201">group</span></span>](../resources/group.md)| <span data-ttu-id="625a0-202">O grupo de diretórios correspondente a esta classe.</span><span class="sxs-lookup"><span data-stu-id="625a0-202">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="625a0-203">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="625a0-203">JSON representation</span></span>

<span data-ttu-id="625a0-204">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="625a0-204">The following is a JSON representation of the resource.</span></span>

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
