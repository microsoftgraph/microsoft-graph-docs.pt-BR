---
title: Tipo de recurso educationSchool
description: 'Uma escola. O recurso **educationSchool** atualmente corresponde a um recurso administrativeUnit e compartilha a mesma ID.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9cded9db9ab9d7310a10ab690e05f49dca8711c8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750140"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="9aa06-104">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="9aa06-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aa06-105">Uma escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-105">A school.</span></span> <span data-ttu-id="9aa06-106">O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="9aa06-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="9aa06-107">Esse recurso é um subtipo de [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="9aa06-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9aa06-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9aa06-108">Methods</span></span>

| <span data-ttu-id="9aa06-109">Método</span><span class="sxs-lookup"><span data-stu-id="9aa06-109">Method</span></span>                                                                     | <span data-ttu-id="9aa06-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9aa06-110">Return Type</span></span>                                      | <span data-ttu-id="9aa06-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aa06-111">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="9aa06-112">Get</span><span class="sxs-lookup"><span data-stu-id="9aa06-112">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="9aa06-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="9aa06-113">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="9aa06-114">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="9aa06-114">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="9aa06-115">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="9aa06-115">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="9aa06-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="9aa06-116">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="9aa06-117">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="9aa06-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="9aa06-118">Listar classes</span><span class="sxs-lookup"><span data-stu-id="9aa06-118">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="9aa06-119">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="9aa06-119">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="9aa06-120">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="9aa06-120">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="9aa06-121">Remover classe</span><span class="sxs-lookup"><span data-stu-id="9aa06-121">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="9aa06-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="9aa06-122">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="9aa06-123">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="9aa06-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="9aa06-124">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="9aa06-124">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="9aa06-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="9aa06-125">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="9aa06-126">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="9aa06-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="9aa06-127">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="9aa06-127">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="9aa06-128">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="9aa06-128">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="9aa06-129">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="9aa06-129">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="9aa06-130">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="9aa06-130">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="9aa06-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="9aa06-131">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="9aa06-132">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="9aa06-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="9aa06-133">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="9aa06-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="9aa06-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="9aa06-134">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="9aa06-135">Obtenha o **administrativeUnit** que corresponde a esse **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="9aa06-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="9aa06-136">Atualizar</span><span class="sxs-lookup"><span data-stu-id="9aa06-136">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="9aa06-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="9aa06-137">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="9aa06-138">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="9aa06-138">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="9aa06-139">Delete</span><span class="sxs-lookup"><span data-stu-id="9aa06-139">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="9aa06-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9aa06-140">None</span></span>                                             | <span data-ttu-id="9aa06-141">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="9aa06-141">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="9aa06-142">Delta</span><span class="sxs-lookup"><span data-stu-id="9aa06-142">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="9aa06-143">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="9aa06-143">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="9aa06-144">Obter alterações incrementais para o **educationSchools**</span><span class="sxs-lookup"><span data-stu-id="9aa06-144">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="9aa06-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9aa06-145">Properties</span></span>

| <span data-ttu-id="9aa06-146">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9aa06-146">Property</span></span>            | <span data-ttu-id="9aa06-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aa06-147">Type</span></span>                                  | <span data-ttu-id="9aa06-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aa06-148">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="9aa06-149">id</span><span class="sxs-lookup"><span data-stu-id="9aa06-149">id</span></span>                  | <span data-ttu-id="9aa06-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9aa06-150">String</span></span>                                | <span data-ttu-id="9aa06-151">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-151">GUID of this school.</span></span>                               |
| <span data-ttu-id="9aa06-152">address</span><span class="sxs-lookup"><span data-stu-id="9aa06-152">address</span></span>             | [<span data-ttu-id="9aa06-153">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9aa06-153">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="9aa06-154">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-154">Address of the school.</span></span>                             |
| <span data-ttu-id="9aa06-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="9aa06-155">createdBy</span></span>           | [<span data-ttu-id="9aa06-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="9aa06-156">identitySet</span></span>](identityset.md)         | <span data-ttu-id="9aa06-157">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-157">Entity who created the school.</span></span>                     |
| <span data-ttu-id="9aa06-158">descrição</span><span class="sxs-lookup"><span data-stu-id="9aa06-158">description</span></span>         | <span data-ttu-id="9aa06-159">String</span><span class="sxs-lookup"><span data-stu-id="9aa06-159">String</span></span>                                | <span data-ttu-id="9aa06-160">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-160">Description of the school.</span></span>                         |
| <span data-ttu-id="9aa06-161">displayName</span><span class="sxs-lookup"><span data-stu-id="9aa06-161">displayName</span></span>         | <span data-ttu-id="9aa06-162">String</span><span class="sxs-lookup"><span data-stu-id="9aa06-162">String</span></span>                                | <span data-ttu-id="9aa06-163">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-163">Display name of the school.</span></span>                        |
| <span data-ttu-id="9aa06-164">externalId</span><span class="sxs-lookup"><span data-stu-id="9aa06-164">externalId</span></span>          | <span data-ttu-id="9aa06-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9aa06-165">String</span></span>                                | <span data-ttu-id="9aa06-166">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="9aa06-166">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="9aa06-167">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="9aa06-167">externalPrincipalId</span></span> | <span data-ttu-id="9aa06-168">String</span><span class="sxs-lookup"><span data-stu-id="9aa06-168">String</span></span>                                | <span data-ttu-id="9aa06-169">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="9aa06-169">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="9aa06-170">externalSource</span><span class="sxs-lookup"><span data-stu-id="9aa06-170">externalSource</span></span>      | <span data-ttu-id="9aa06-171">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9aa06-171">string</span></span>                                | <span data-ttu-id="9aa06-172">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="9aa06-172">Read-Only.</span></span> <span data-ttu-id="9aa06-173">Os valores possíveis são: `sis` ou `manual`.</span><span class="sxs-lookup"><span data-stu-id="9aa06-173">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="9aa06-174">fax</span><span class="sxs-lookup"><span data-stu-id="9aa06-174">fax</span></span>                 | <span data-ttu-id="9aa06-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9aa06-175">String</span></span>                                | <span data-ttu-id="9aa06-176">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-176">Fax number of school.</span></span>                              |
| <span data-ttu-id="9aa06-177">highestGrade</span><span class="sxs-lookup"><span data-stu-id="9aa06-177">highestGrade</span></span>        | <span data-ttu-id="9aa06-178">String</span><span class="sxs-lookup"><span data-stu-id="9aa06-178">String</span></span>                                | <span data-ttu-id="9aa06-179">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="9aa06-179">Highest grade taught.</span></span>                              |
| <span data-ttu-id="9aa06-180">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="9aa06-180">lowestGrade</span></span>         | <span data-ttu-id="9aa06-181">String</span><span class="sxs-lookup"><span data-stu-id="9aa06-181">String</span></span>                                | <span data-ttu-id="9aa06-182">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="9aa06-182">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="9aa06-183">phone</span><span class="sxs-lookup"><span data-stu-id="9aa06-183">phone</span></span>               | <span data-ttu-id="9aa06-184">String</span><span class="sxs-lookup"><span data-stu-id="9aa06-184">String</span></span>                                | <span data-ttu-id="9aa06-185">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-185">Phone number of school.</span></span>                            |
| <span data-ttu-id="9aa06-186">principalEmail</span><span class="sxs-lookup"><span data-stu-id="9aa06-186">principalEmail</span></span>      | <span data-ttu-id="9aa06-187">String</span><span class="sxs-lookup"><span data-stu-id="9aa06-187">String</span></span>                                | <span data-ttu-id="9aa06-188">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="9aa06-188">Email address of the principal.</span></span>                    |
| <span data-ttu-id="9aa06-189">principalName</span><span class="sxs-lookup"><span data-stu-id="9aa06-189">principalName</span></span>       | <span data-ttu-id="9aa06-190">String</span><span class="sxs-lookup"><span data-stu-id="9aa06-190">String</span></span>                                | <span data-ttu-id="9aa06-191">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="9aa06-191">Name of the principal.</span></span>                             |
| <span data-ttu-id="9aa06-192">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="9aa06-192">schoolNumber</span></span>        | <span data-ttu-id="9aa06-193">String</span><span class="sxs-lookup"><span data-stu-id="9aa06-193">String</span></span>                                | <span data-ttu-id="9aa06-194">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-194">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="9aa06-195">Relações</span><span class="sxs-lookup"><span data-stu-id="9aa06-195">Relationships</span></span>

| <span data-ttu-id="9aa06-196">Relação</span><span class="sxs-lookup"><span data-stu-id="9aa06-196">Relationship</span></span> | <span data-ttu-id="9aa06-197">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aa06-197">Type</span></span>                                           | <span data-ttu-id="9aa06-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aa06-198">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="9aa06-199">classes</span><span class="sxs-lookup"><span data-stu-id="9aa06-199">classes</span></span>      | <span data-ttu-id="9aa06-200">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="9aa06-200">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="9aa06-201">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-201">Classes taught at the school.</span></span> <span data-ttu-id="9aa06-202">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9aa06-202">Nullable.</span></span> |
| <span data-ttu-id="9aa06-203">users</span><span class="sxs-lookup"><span data-stu-id="9aa06-203">users</span></span>        | <span data-ttu-id="9aa06-204">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="9aa06-204">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="9aa06-205">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="9aa06-205">Users in the school.</span></span> <span data-ttu-id="9aa06-206">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9aa06-206">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="9aa06-207">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9aa06-207">JSON representation</span></span>

<span data-ttu-id="9aa06-208">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9aa06-208">The following is a JSON representation of the resource.</span></span>

<!-- {
"blockType": "resource",
"keyProperty": "id",
"optionalProperties": [

],
"@odata.type": "microsoft.graph.educationSchool"
}-->


```json
{
  "address": { "@odata.type": "microsoft.graph.physicalAddress" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalPrincipalId": "String",
  "externalSource": "string",
  "fax": "String",
  "highestGrade": "String",
  "id": "String (identifier)",
  "lowestGrade": "String",
  "phone": "String",
  "principalEmail": "String",
  "principalName": "String",
  "schoolNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource educationSchool has documented navigation properties, but we thought it was a complex type!" 
  ]  
}-->
