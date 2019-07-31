---
title: Tipo de recurso educationSchool
description: 'Uma escola. O recurso **educationSchool** atualmente corresponde a um recurso administrativeUnit e compartilha a mesma ID.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1b5e0807ae73110a921c70beef6a98589db41269
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972548"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="96f81-104">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="96f81-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96f81-105">Uma escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-105">A school.</span></span> <span data-ttu-id="96f81-106">O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="96f81-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="96f81-107">Esse recurso é um subtipo de [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="96f81-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="96f81-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="96f81-108">Methods</span></span>

| <span data-ttu-id="96f81-109">Método</span><span class="sxs-lookup"><span data-stu-id="96f81-109">Method</span></span>                                                                     | <span data-ttu-id="96f81-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="96f81-110">Return Type</span></span>                                      | <span data-ttu-id="96f81-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="96f81-111">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="96f81-112">Get</span><span class="sxs-lookup"><span data-stu-id="96f81-112">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="96f81-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="96f81-113">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="96f81-114">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="96f81-114">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="96f81-115">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="96f81-115">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="96f81-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="96f81-116">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="96f81-117">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="96f81-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="96f81-118">Listar classes</span><span class="sxs-lookup"><span data-stu-id="96f81-118">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="96f81-119">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="96f81-119">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="96f81-120">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="96f81-120">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="96f81-121">Remover classe</span><span class="sxs-lookup"><span data-stu-id="96f81-121">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="96f81-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="96f81-122">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="96f81-123">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="96f81-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="96f81-124">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="96f81-124">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="96f81-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="96f81-125">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="96f81-126">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="96f81-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="96f81-127">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="96f81-127">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="96f81-128">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="96f81-128">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="96f81-129">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="96f81-129">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="96f81-130">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="96f81-130">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="96f81-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="96f81-131">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="96f81-132">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="96f81-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="96f81-133">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="96f81-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="96f81-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="96f81-134">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="96f81-135">Obtenha o **administrativeUnit** que corresponde a esse **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="96f81-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="96f81-136">Atualizar</span><span class="sxs-lookup"><span data-stu-id="96f81-136">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="96f81-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="96f81-137">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="96f81-138">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="96f81-138">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="96f81-139">Delete</span><span class="sxs-lookup"><span data-stu-id="96f81-139">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="96f81-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96f81-140">None</span></span>                                             | <span data-ttu-id="96f81-141">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="96f81-141">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="96f81-142">Delta</span><span class="sxs-lookup"><span data-stu-id="96f81-142">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="96f81-143">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="96f81-143">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="96f81-144">Obter alterações incrementais para o **educationSchools**</span><span class="sxs-lookup"><span data-stu-id="96f81-144">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="96f81-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96f81-145">Properties</span></span>

| <span data-ttu-id="96f81-146">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96f81-146">Property</span></span>            | <span data-ttu-id="96f81-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="96f81-147">Type</span></span>                                  | <span data-ttu-id="96f81-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="96f81-148">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="96f81-149">id</span><span class="sxs-lookup"><span data-stu-id="96f81-149">id</span></span>                  | <span data-ttu-id="96f81-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96f81-150">String</span></span>                                | <span data-ttu-id="96f81-151">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-151">GUID of this school.</span></span>                               |
| <span data-ttu-id="96f81-152">address</span><span class="sxs-lookup"><span data-stu-id="96f81-152">address</span></span>             | [<span data-ttu-id="96f81-153">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="96f81-153">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="96f81-154">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-154">Address of the school.</span></span>                             |
| <span data-ttu-id="96f81-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="96f81-155">createdBy</span></span>           | [<span data-ttu-id="96f81-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="96f81-156">identitySet</span></span>](identityset.md)         | <span data-ttu-id="96f81-157">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-157">Entity who created the school.</span></span>                     |
| <span data-ttu-id="96f81-158">descrição</span><span class="sxs-lookup"><span data-stu-id="96f81-158">description</span></span>         | <span data-ttu-id="96f81-159">String</span><span class="sxs-lookup"><span data-stu-id="96f81-159">String</span></span>                                | <span data-ttu-id="96f81-160">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-160">Description of the school.</span></span>                         |
| <span data-ttu-id="96f81-161">displayName</span><span class="sxs-lookup"><span data-stu-id="96f81-161">displayName</span></span>         | <span data-ttu-id="96f81-162">String</span><span class="sxs-lookup"><span data-stu-id="96f81-162">String</span></span>                                | <span data-ttu-id="96f81-163">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-163">Display name of the school.</span></span>                        |
| <span data-ttu-id="96f81-164">externalId</span><span class="sxs-lookup"><span data-stu-id="96f81-164">externalId</span></span>          | <span data-ttu-id="96f81-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96f81-165">String</span></span>                                | <span data-ttu-id="96f81-166">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="96f81-166">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="96f81-167">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="96f81-167">externalPrincipalId</span></span> | <span data-ttu-id="96f81-168">String</span><span class="sxs-lookup"><span data-stu-id="96f81-168">String</span></span>                                | <span data-ttu-id="96f81-169">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="96f81-169">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="96f81-170">externalSource</span><span class="sxs-lookup"><span data-stu-id="96f81-170">externalSource</span></span>      | <span data-ttu-id="96f81-171">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96f81-171">string</span></span>                                | <span data-ttu-id="96f81-172">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="96f81-172">Read-Only.</span></span> <span data-ttu-id="96f81-173">Os valores possíveis são: `sis` ou `manual`.</span><span class="sxs-lookup"><span data-stu-id="96f81-173">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="96f81-174">fax</span><span class="sxs-lookup"><span data-stu-id="96f81-174">fax</span></span>                 | <span data-ttu-id="96f81-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96f81-175">String</span></span>                                | <span data-ttu-id="96f81-176">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-176">Fax number of school.</span></span>                              |
| <span data-ttu-id="96f81-177">highestGrade</span><span class="sxs-lookup"><span data-stu-id="96f81-177">highestGrade</span></span>        | <span data-ttu-id="96f81-178">String</span><span class="sxs-lookup"><span data-stu-id="96f81-178">String</span></span>                                | <span data-ttu-id="96f81-179">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="96f81-179">Highest grade taught.</span></span>                              |
| <span data-ttu-id="96f81-180">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="96f81-180">lowestGrade</span></span>         | <span data-ttu-id="96f81-181">String</span><span class="sxs-lookup"><span data-stu-id="96f81-181">String</span></span>                                | <span data-ttu-id="96f81-182">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="96f81-182">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="96f81-183">phone</span><span class="sxs-lookup"><span data-stu-id="96f81-183">phone</span></span>               | <span data-ttu-id="96f81-184">String</span><span class="sxs-lookup"><span data-stu-id="96f81-184">String</span></span>                                | <span data-ttu-id="96f81-185">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-185">Phone number of school.</span></span>                            |
| <span data-ttu-id="96f81-186">principalEmail</span><span class="sxs-lookup"><span data-stu-id="96f81-186">principalEmail</span></span>      | <span data-ttu-id="96f81-187">String</span><span class="sxs-lookup"><span data-stu-id="96f81-187">String</span></span>                                | <span data-ttu-id="96f81-188">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="96f81-188">Email address of the principal.</span></span>                    |
| <span data-ttu-id="96f81-189">principalName</span><span class="sxs-lookup"><span data-stu-id="96f81-189">principalName</span></span>       | <span data-ttu-id="96f81-190">String</span><span class="sxs-lookup"><span data-stu-id="96f81-190">String</span></span>                                | <span data-ttu-id="96f81-191">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="96f81-191">Name of the principal.</span></span>                             |
| <span data-ttu-id="96f81-192">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="96f81-192">schoolNumber</span></span>        | <span data-ttu-id="96f81-193">String</span><span class="sxs-lookup"><span data-stu-id="96f81-193">String</span></span>                                | <span data-ttu-id="96f81-194">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-194">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="96f81-195">Relações</span><span class="sxs-lookup"><span data-stu-id="96f81-195">Relationships</span></span>

| <span data-ttu-id="96f81-196">Relação</span><span class="sxs-lookup"><span data-stu-id="96f81-196">Relationship</span></span> | <span data-ttu-id="96f81-197">Tipo</span><span class="sxs-lookup"><span data-stu-id="96f81-197">Type</span></span>                                           | <span data-ttu-id="96f81-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="96f81-198">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="96f81-199">classes</span><span class="sxs-lookup"><span data-stu-id="96f81-199">classes</span></span>      | <span data-ttu-id="96f81-200">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="96f81-200">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="96f81-201">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-201">Classes taught at the school.</span></span> <span data-ttu-id="96f81-202">Anulável.</span><span class="sxs-lookup"><span data-stu-id="96f81-202">Nullable.</span></span> |
| <span data-ttu-id="96f81-203">users</span><span class="sxs-lookup"><span data-stu-id="96f81-203">users</span></span>        | <span data-ttu-id="96f81-204">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="96f81-204">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="96f81-205">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="96f81-205">Users in the school.</span></span> <span data-ttu-id="96f81-206">Anulável.</span><span class="sxs-lookup"><span data-stu-id="96f81-206">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="96f81-207">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96f81-207">JSON representation</span></span>

<span data-ttu-id="96f81-208">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96f81-208">The following is a JSON representation of the resource.</span></span>

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
