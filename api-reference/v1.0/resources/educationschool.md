# <a name="educationschool-resource-type"></a><span data-ttu-id="fd65f-101">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="fd65f-101">educationSchool resource type</span></span>

<span data-ttu-id="fd65f-102">Recurso usado para gerenciar aulas, professores e alunos da escola representada.</span><span class="sxs-lookup"><span data-stu-id="fd65f-102">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="fd65f-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="fd65f-103">Methods</span></span>

| <span data-ttu-id="fd65f-104">Método</span><span class="sxs-lookup"><span data-stu-id="fd65f-104">Method</span></span>           | <span data-ttu-id="fd65f-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fd65f-105">Return Type</span></span>    |<span data-ttu-id="fd65f-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd65f-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd65f-107">Obter</span><span class="sxs-lookup"><span data-stu-id="fd65f-107">Get</span></span>](../api/educationschool_get.md) | [<span data-ttu-id="fd65f-108">educationSchool</span><span class="sxs-lookup"><span data-stu-id="fd65f-108">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="fd65f-109">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="fd65f-109">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="fd65f-110">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="fd65f-110">Add class</span></span>](../api/educationschool_post_classes.md) |[<span data-ttu-id="fd65f-111">educationClass</span><span class="sxs-lookup"><span data-stu-id="fd65f-111">educationClass</span></span>](educationclass.md)| <span data-ttu-id="fd65f-112">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="fd65f-112">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="fd65f-113">Listar classes</span><span class="sxs-lookup"><span data-stu-id="fd65f-113">List classes</span></span>](../api/educationschool_list_classes.md) |<span data-ttu-id="fd65f-114">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="fd65f-114">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="fd65f-115">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="fd65f-115">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="fd65f-116">Remover classe</span><span class="sxs-lookup"><span data-stu-id="fd65f-116">Remove class</span></span>](../api/educationschool_delete_classes.md) |[<span data-ttu-id="fd65f-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="fd65f-117">educationClass</span></span>](educationclass.md)| <span data-ttu-id="fd65f-118">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="fd65f-118">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="fd65f-119">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="fd65f-119">Add user</span></span>](../api/educationschool_post_users.md) |[<span data-ttu-id="fd65f-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="fd65f-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="fd65f-121">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="fd65f-121">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="fd65f-122">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="fd65f-122">List users</span></span>](../api/educationschool_list_users.md) |<span data-ttu-id="fd65f-123">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="fd65f-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="fd65f-124">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="fd65f-124">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="fd65f-125">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="fd65f-125">Remove user</span></span>](../api/educationschool_delete_users.md) |[<span data-ttu-id="fd65f-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="fd65f-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="fd65f-127">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="fd65f-127">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="fd65f-128">Atualizar</span><span class="sxs-lookup"><span data-stu-id="fd65f-128">Update</span></span>](../api/educationschool_update.md) | [<span data-ttu-id="fd65f-129">educationSchool</span><span class="sxs-lookup"><span data-stu-id="fd65f-129">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="fd65f-130">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="fd65f-130">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="fd65f-131">Excluir</span><span class="sxs-lookup"><span data-stu-id="fd65f-131">Delete</span></span>](../api/educationschool_delete.md) | <span data-ttu-id="fd65f-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd65f-132">None</span></span> |<span data-ttu-id="fd65f-133">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="fd65f-133">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fd65f-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd65f-134">Properties</span></span>
| <span data-ttu-id="fd65f-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd65f-135">Property</span></span>     | <span data-ttu-id="fd65f-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd65f-136">Type</span></span>   |<span data-ttu-id="fd65f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd65f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd65f-138">id</span><span class="sxs-lookup"><span data-stu-id="fd65f-138">id</span></span>|<span data-ttu-id="fd65f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-139">String</span></span>|<span data-ttu-id="fd65f-140">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-140">GUID of this school.</span></span>|
|<span data-ttu-id="fd65f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="fd65f-141">displayName</span></span>| <span data-ttu-id="fd65f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-142">String</span></span>| <span data-ttu-id="fd65f-143">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-143">Display name of the school.</span></span>| 
|<span data-ttu-id="fd65f-144">description</span><span class="sxs-lookup"><span data-stu-id="fd65f-144">description</span></span>| <span data-ttu-id="fd65f-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-145">String</span></span> | <span data-ttu-id="fd65f-146">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-146">Description of the school.</span></span>| 
|<span data-ttu-id="fd65f-147">status</span><span class="sxs-lookup"><span data-stu-id="fd65f-147">status</span></span>| <span data-ttu-id="fd65f-148">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-148">string</span></span>| <span data-ttu-id="fd65f-149">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="fd65f-149">Read-Only.</span></span> <span data-ttu-id="fd65f-150">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="fd65f-150">The possible values are `inactive`, `active`, `expired`, `deleteable`, , , , , , , , or .</span></span>|
|<span data-ttu-id="fd65f-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="fd65f-151">externalSource</span></span>| <span data-ttu-id="fd65f-152">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="fd65f-152">educationExternalSource</span></span>| <span data-ttu-id="fd65f-153">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="fd65f-153">Read-Only.</span></span>  <span data-ttu-id="fd65f-154">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fd65f-154">The possible values are:</span></span>|
|<span data-ttu-id="fd65f-155">principalEmail</span><span class="sxs-lookup"><span data-stu-id="fd65f-155">principalEmail</span></span>| <span data-ttu-id="fd65f-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-156">String</span></span>| <span data-ttu-id="fd65f-157">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="fd65f-157">Email address of the principal.</span></span>|
|<span data-ttu-id="fd65f-158">principalName</span><span class="sxs-lookup"><span data-stu-id="fd65f-158">principalName</span></span>| <span data-ttu-id="fd65f-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-159">String</span></span> | <span data-ttu-id="fd65f-160">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="fd65f-160">Name of the principal.</span></span>|
|<span data-ttu-id="fd65f-161">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="fd65f-161">externalPrincipalId</span></span>| <span data-ttu-id="fd65f-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-162">String</span></span> | <span data-ttu-id="fd65f-163">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fd65f-163">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="fd65f-164">highestGrade</span><span class="sxs-lookup"><span data-stu-id="fd65f-164">highestGrade</span></span>|<span data-ttu-id="fd65f-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-165">String</span></span>| <span data-ttu-id="fd65f-166">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="fd65f-166">Highest grade taught.</span></span> |
|<span data-ttu-id="fd65f-167">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="fd65f-167">lowestGrade</span></span>|<span data-ttu-id="fd65f-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-168">String</span></span>| <span data-ttu-id="fd65f-169">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="fd65f-169">Lowest grade taught.</span></span> |
|<span data-ttu-id="fd65f-170">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="fd65f-170">schoolNumber</span></span>|<span data-ttu-id="fd65f-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-171">String</span></span>| <span data-ttu-id="fd65f-172">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-172">School Number.</span></span>|
|<span data-ttu-id="fd65f-173">externalId</span><span class="sxs-lookup"><span data-stu-id="fd65f-173">externalId</span></span>|<span data-ttu-id="fd65f-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-174">String</span></span>| <span data-ttu-id="fd65f-175">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fd65f-175">ID of school in syncing system.</span></span> |
|<span data-ttu-id="fd65f-176">phone</span><span class="sxs-lookup"><span data-stu-id="fd65f-176">phone</span></span>|<span data-ttu-id="fd65f-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-177">String</span></span>| <span data-ttu-id="fd65f-178">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-178">Phone number of school.</span></span> |
|<span data-ttu-id="fd65f-179">fax</span><span class="sxs-lookup"><span data-stu-id="fd65f-179">fax</span></span>|<span data-ttu-id="fd65f-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd65f-180">String</span></span>| <span data-ttu-id="fd65f-181">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-181">Fax number of school.</span></span> |
|<span data-ttu-id="fd65f-182">address</span><span class="sxs-lookup"><span data-stu-id="fd65f-182">address</span></span>|[<span data-ttu-id="fd65f-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="fd65f-183">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="fd65f-184">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-184">Address of the school.</span></span>|
|<span data-ttu-id="fd65f-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="fd65f-185">createdBy</span></span>|[<span data-ttu-id="fd65f-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="fd65f-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="fd65f-187">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-187">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd65f-188">Relações</span><span class="sxs-lookup"><span data-stu-id="fd65f-188">Relationships</span></span>
| <span data-ttu-id="fd65f-189">Relação</span><span class="sxs-lookup"><span data-stu-id="fd65f-189">Relationship</span></span> | <span data-ttu-id="fd65f-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd65f-190">Type</span></span>   |<span data-ttu-id="fd65f-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd65f-191">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd65f-192">classes</span><span class="sxs-lookup"><span data-stu-id="fd65f-192">classes</span></span>|<span data-ttu-id="fd65f-193">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="fd65f-193">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="fd65f-194">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-194">Classes taught at the school.</span></span> <span data-ttu-id="fd65f-195">Anulável.</span><span class="sxs-lookup"><span data-stu-id="fd65f-195">Nullable.</span></span>|
|<span data-ttu-id="fd65f-196">users</span><span class="sxs-lookup"><span data-stu-id="fd65f-196">users</span></span>|<span data-ttu-id="fd65f-197">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="fd65f-197">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="fd65f-198">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="fd65f-198">Users in the school.</span></span> <span data-ttu-id="fd65f-199">Anulável.</span><span class="sxs-lookup"><span data-stu-id="fd65f-199">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd65f-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd65f-200">JSON representation</span></span>

<span data-ttu-id="fd65f-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd65f-201">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
