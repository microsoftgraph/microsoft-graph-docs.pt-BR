---
title: Tipo de recurso educationSchool
description: 'Escola A. O recurso **educationSchool** atualmente corresponde a um recurso administrativeUnit e compartilha a mesma ID.  '
localization_priority: Normal
ms.openlocfilehash: 20eacb87b68cbf490131b98a15d3ab3239d73478
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830447"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="d0284-104">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="d0284-104">educationSchool resource type</span></span>

> <span data-ttu-id="d0284-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d0284-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0284-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d0284-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0284-107">Escola A.</span><span class="sxs-lookup"><span data-stu-id="d0284-107">A school.</span></span> <span data-ttu-id="d0284-108">O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="d0284-108">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="d0284-109">Esse recurso é um subtipo de [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="d0284-109">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="d0284-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="d0284-110">Methods</span></span>

| <span data-ttu-id="d0284-111">Método</span><span class="sxs-lookup"><span data-stu-id="d0284-111">Method</span></span>           | <span data-ttu-id="d0284-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d0284-112">Return Type</span></span>    |<span data-ttu-id="d0284-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0284-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d0284-114">Obter</span><span class="sxs-lookup"><span data-stu-id="d0284-114">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="d0284-115">educationSchool</span><span class="sxs-lookup"><span data-stu-id="d0284-115">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="d0284-116">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="d0284-116">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="d0284-117">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="d0284-117">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="d0284-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="d0284-118">educationClass</span></span>](educationclass.md)| <span data-ttu-id="d0284-119">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="d0284-119">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="d0284-120">Listar classes</span><span class="sxs-lookup"><span data-stu-id="d0284-120">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="d0284-121">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="d0284-121">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="d0284-122">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="d0284-122">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="d0284-123">Remover classe</span><span class="sxs-lookup"><span data-stu-id="d0284-123">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="d0284-124">educationClass</span><span class="sxs-lookup"><span data-stu-id="d0284-124">educationClass</span></span>](educationclass.md)| <span data-ttu-id="d0284-125">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="d0284-125">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="d0284-126">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="d0284-126">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="d0284-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="d0284-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="d0284-128">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="d0284-128">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="d0284-129">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="d0284-129">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="d0284-130">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="d0284-130">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="d0284-131">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="d0284-131">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="d0284-132">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="d0284-132">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="d0284-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="d0284-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="d0284-134">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="d0284-134">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="d0284-135">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="d0284-135">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="d0284-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="d0284-136">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="d0284-137">Obtenha a **administrativeUnit** que corresponde a essa **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="d0284-137">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="d0284-138">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d0284-138">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="d0284-139">educationSchool</span><span class="sxs-lookup"><span data-stu-id="d0284-139">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="d0284-140">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="d0284-140">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="d0284-141">Excluir</span><span class="sxs-lookup"><span data-stu-id="d0284-141">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="d0284-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0284-142">None</span></span> |<span data-ttu-id="d0284-143">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="d0284-143">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d0284-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0284-144">Properties</span></span>
| <span data-ttu-id="d0284-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0284-145">Property</span></span>     | <span data-ttu-id="d0284-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0284-146">Type</span></span>   |<span data-ttu-id="d0284-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0284-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0284-148">id</span><span class="sxs-lookup"><span data-stu-id="d0284-148">id</span></span>|<span data-ttu-id="d0284-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-149">String</span></span>|<span data-ttu-id="d0284-150">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-150">GUID of this school.</span></span>|
|<span data-ttu-id="d0284-151">displayName</span><span class="sxs-lookup"><span data-stu-id="d0284-151">displayName</span></span>| <span data-ttu-id="d0284-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-152">String</span></span>| <span data-ttu-id="d0284-153">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-153">Display name of the school.</span></span>| 
|<span data-ttu-id="d0284-154">description</span><span class="sxs-lookup"><span data-stu-id="d0284-154">description</span></span>| <span data-ttu-id="d0284-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-155">String</span></span> | <span data-ttu-id="d0284-156">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-156">Description of the school.</span></span>| 
|<span data-ttu-id="d0284-157">status</span><span class="sxs-lookup"><span data-stu-id="d0284-157">status</span></span>| <span data-ttu-id="d0284-158">string</span><span class="sxs-lookup"><span data-stu-id="d0284-158">string</span></span>| <span data-ttu-id="d0284-159">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="d0284-159">Read-Only.</span></span> <span data-ttu-id="d0284-160">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="d0284-160">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="d0284-161">externalSource</span><span class="sxs-lookup"><span data-stu-id="d0284-161">externalSource</span></span>| <span data-ttu-id="d0284-162">string</span><span class="sxs-lookup"><span data-stu-id="d0284-162">string</span></span>| <span data-ttu-id="d0284-163">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="d0284-163">Read-Only.</span></span>  <span data-ttu-id="d0284-164">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d0284-164">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d0284-165">principalEmail</span><span class="sxs-lookup"><span data-stu-id="d0284-165">principalEmail</span></span>| <span data-ttu-id="d0284-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-166">String</span></span>| <span data-ttu-id="d0284-167">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="d0284-167">Email address of the principal.</span></span>|
|<span data-ttu-id="d0284-168">principalName</span><span class="sxs-lookup"><span data-stu-id="d0284-168">principalName</span></span>| <span data-ttu-id="d0284-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-169">String</span></span> | <span data-ttu-id="d0284-170">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="d0284-170">Name of the principal.</span></span>|
|<span data-ttu-id="d0284-171">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="d0284-171">externalPrincipalId</span></span>| <span data-ttu-id="d0284-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-172">String</span></span> | <span data-ttu-id="d0284-173">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="d0284-173">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="d0284-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="d0284-174">highestGrade</span></span>|<span data-ttu-id="d0284-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-175">String</span></span>| <span data-ttu-id="d0284-176">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="d0284-176">Highest grade taught.</span></span> |
|<span data-ttu-id="d0284-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="d0284-177">lowestGrade</span></span>|<span data-ttu-id="d0284-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-178">String</span></span>| <span data-ttu-id="d0284-179">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="d0284-179">Lowest grade taught.</span></span> |
|<span data-ttu-id="d0284-180">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="d0284-180">schoolNumber</span></span>|<span data-ttu-id="d0284-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-181">String</span></span>| <span data-ttu-id="d0284-182">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-182">School Number.</span></span>|
|<span data-ttu-id="d0284-183">externalId</span><span class="sxs-lookup"><span data-stu-id="d0284-183">externalId</span></span>|<span data-ttu-id="d0284-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-184">String</span></span>| <span data-ttu-id="d0284-185">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="d0284-185">ID of school in syncing system.</span></span> |
|<span data-ttu-id="d0284-186">phone</span><span class="sxs-lookup"><span data-stu-id="d0284-186">phone</span></span>|<span data-ttu-id="d0284-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-187">String</span></span>| <span data-ttu-id="d0284-188">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-188">Phone number of school.</span></span> |
|<span data-ttu-id="d0284-189">fax</span><span class="sxs-lookup"><span data-stu-id="d0284-189">fax</span></span>|<span data-ttu-id="d0284-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0284-190">String</span></span>| <span data-ttu-id="d0284-191">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-191">Fax number of school.</span></span> |
|<span data-ttu-id="d0284-192">address</span><span class="sxs-lookup"><span data-stu-id="d0284-192">address</span></span>|[<span data-ttu-id="d0284-193">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d0284-193">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="d0284-194">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-194">Address of the school.</span></span>|
|<span data-ttu-id="d0284-195">createdBy</span><span class="sxs-lookup"><span data-stu-id="d0284-195">createdBy</span></span>|[<span data-ttu-id="d0284-196">identitySet</span><span class="sxs-lookup"><span data-stu-id="d0284-196">identitySet</span></span>](identityset.md)|<span data-ttu-id="d0284-197">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-197">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d0284-198">Relações</span><span class="sxs-lookup"><span data-stu-id="d0284-198">Relationships</span></span>
| <span data-ttu-id="d0284-199">Relação</span><span class="sxs-lookup"><span data-stu-id="d0284-199">Relationship</span></span> | <span data-ttu-id="d0284-200">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0284-200">Type</span></span>   |<span data-ttu-id="d0284-201">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0284-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0284-202">classes</span><span class="sxs-lookup"><span data-stu-id="d0284-202">classes</span></span>|<span data-ttu-id="d0284-203">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="d0284-203">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="d0284-204">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-204">Classes taught at the school.</span></span> <span data-ttu-id="d0284-205">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d0284-205">Nullable.</span></span>|
|<span data-ttu-id="d0284-206">users</span><span class="sxs-lookup"><span data-stu-id="d0284-206">users</span></span>|<span data-ttu-id="d0284-207">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="d0284-207">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="d0284-208">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="d0284-208">Users in the school.</span></span> <span data-ttu-id="d0284-209">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d0284-209">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0284-210">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0284-210">JSON representation</span></span>

<span data-ttu-id="d0284-211">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0284-211">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
