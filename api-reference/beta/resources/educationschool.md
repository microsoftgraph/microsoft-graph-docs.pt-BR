---
title: Tipo de recurso educationSchool
description: 'Uma escola. O recurso **educationSchool** atualmente corresponde a um recurso administrativeUnit e compartilha a mesma ID.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 208527c1b846a307b88e3f96204dba660caedb9a
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909548"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="991ce-104">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="991ce-104">educationSchool resource type</span></span>

<span data-ttu-id="991ce-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="991ce-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="991ce-106">Uma escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-106">A school.</span></span> <span data-ttu-id="991ce-107">O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="991ce-107">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="991ce-108">Esse recurso é um subtipo de [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="991ce-108">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="991ce-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="991ce-109">Methods</span></span>

| <span data-ttu-id="991ce-110">Método</span><span class="sxs-lookup"><span data-stu-id="991ce-110">Method</span></span>                                                                     | <span data-ttu-id="991ce-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="991ce-111">Return Type</span></span>                                      | <span data-ttu-id="991ce-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="991ce-112">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="991ce-113">Get</span><span class="sxs-lookup"><span data-stu-id="991ce-113">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="991ce-114">educationSchool</span><span class="sxs-lookup"><span data-stu-id="991ce-114">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="991ce-115">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="991ce-115">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="991ce-116">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="991ce-116">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="991ce-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="991ce-117">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="991ce-118">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="991ce-118">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="991ce-119">Listar classes</span><span class="sxs-lookup"><span data-stu-id="991ce-119">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="991ce-120">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="991ce-120">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="991ce-121">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="991ce-121">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="991ce-122">Remover classe</span><span class="sxs-lookup"><span data-stu-id="991ce-122">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="991ce-123">educationClass</span><span class="sxs-lookup"><span data-stu-id="991ce-123">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="991ce-124">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="991ce-124">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="991ce-125">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="991ce-125">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="991ce-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="991ce-126">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="991ce-127">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="991ce-127">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="991ce-128">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="991ce-128">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="991ce-129">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="991ce-129">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="991ce-130">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="991ce-130">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="991ce-131">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="991ce-131">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="991ce-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="991ce-132">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="991ce-133">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="991ce-133">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="991ce-134">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="991ce-134">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="991ce-135">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="991ce-135">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="991ce-136">Obtenha o **administrativeUnit** que corresponde a esse **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="991ce-136">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="991ce-137">Atualizar</span><span class="sxs-lookup"><span data-stu-id="991ce-137">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="991ce-138">educationSchool</span><span class="sxs-lookup"><span data-stu-id="991ce-138">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="991ce-139">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="991ce-139">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="991ce-140">Delete</span><span class="sxs-lookup"><span data-stu-id="991ce-140">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="991ce-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="991ce-141">None</span></span>                                             | <span data-ttu-id="991ce-142">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="991ce-142">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="991ce-143">Delta</span><span class="sxs-lookup"><span data-stu-id="991ce-143">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="991ce-144">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="991ce-144">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="991ce-145">Obter alterações incrementais para o **educationSchools**</span><span class="sxs-lookup"><span data-stu-id="991ce-145">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="991ce-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="991ce-146">Properties</span></span>

| <span data-ttu-id="991ce-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="991ce-147">Property</span></span>            | <span data-ttu-id="991ce-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="991ce-148">Type</span></span>                                  | <span data-ttu-id="991ce-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="991ce-149">Description</span></span>                                               |
| :------------------ | :------------------------------------ | :-------------------------------------------------------- |
| <span data-ttu-id="991ce-150">id</span><span class="sxs-lookup"><span data-stu-id="991ce-150">id</span></span>                  | <span data-ttu-id="991ce-151">String</span><span class="sxs-lookup"><span data-stu-id="991ce-151">String</span></span>                                | <span data-ttu-id="991ce-152">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-152">GUID of this school.</span></span>                                      |
| <span data-ttu-id="991ce-153">address</span><span class="sxs-lookup"><span data-stu-id="991ce-153">address</span></span>             | [<span data-ttu-id="991ce-154">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="991ce-154">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="991ce-155">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-155">Address of the school.</span></span>                                    |
| <span data-ttu-id="991ce-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="991ce-156">createdBy</span></span>           | [<span data-ttu-id="991ce-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="991ce-157">identitySet</span></span>](identityset.md)         | <span data-ttu-id="991ce-158">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-158">Entity who created the school.</span></span>                            |
| <span data-ttu-id="991ce-159">description</span><span class="sxs-lookup"><span data-stu-id="991ce-159">description</span></span>         | <span data-ttu-id="991ce-160">String</span><span class="sxs-lookup"><span data-stu-id="991ce-160">String</span></span>                                | <span data-ttu-id="991ce-161">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-161">Description of the school.</span></span>                                |
| <span data-ttu-id="991ce-162">displayName</span><span class="sxs-lookup"><span data-stu-id="991ce-162">displayName</span></span>         | <span data-ttu-id="991ce-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="991ce-163">String</span></span>                                | <span data-ttu-id="991ce-164">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-164">Display name of the school.</span></span>                               |
| <span data-ttu-id="991ce-165">externalId</span><span class="sxs-lookup"><span data-stu-id="991ce-165">externalId</span></span>          | <span data-ttu-id="991ce-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="991ce-166">String</span></span>                                | <span data-ttu-id="991ce-167">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="991ce-167">ID of school in syncing system.</span></span>                           |
| <span data-ttu-id="991ce-168">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="991ce-168">externalPrincipalId</span></span> | <span data-ttu-id="991ce-169">String</span><span class="sxs-lookup"><span data-stu-id="991ce-169">String</span></span>                                | <span data-ttu-id="991ce-170">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="991ce-170">ID of principal in syncing system.</span></span>                        |
| <span data-ttu-id="991ce-171">externalSource</span><span class="sxs-lookup"><span data-stu-id="991ce-171">externalSource</span></span>      | <span data-ttu-id="991ce-172">String</span><span class="sxs-lookup"><span data-stu-id="991ce-172">String</span></span>                                | <span data-ttu-id="991ce-173">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="991ce-173">Read-Only.</span></span> <span data-ttu-id="991ce-174">Os valores possíveis são: `sis` , `lms` ou `manual` .</span><span class="sxs-lookup"><span data-stu-id="991ce-174">Possible values are: `sis`, `lms` or `manual`.</span></span> |
| <span data-ttu-id="991ce-175">highestGrade</span><span class="sxs-lookup"><span data-stu-id="991ce-175">highestGrade</span></span>        | <span data-ttu-id="991ce-176">String</span><span class="sxs-lookup"><span data-stu-id="991ce-176">String</span></span>                                | <span data-ttu-id="991ce-177">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="991ce-177">Highest grade taught.</span></span>                                     |
| <span data-ttu-id="991ce-178">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="991ce-178">lowestGrade</span></span>         | <span data-ttu-id="991ce-179">String</span><span class="sxs-lookup"><span data-stu-id="991ce-179">String</span></span>                                | <span data-ttu-id="991ce-180">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="991ce-180">Lowest grade taught.</span></span>                                      |
| <span data-ttu-id="991ce-181">phone</span><span class="sxs-lookup"><span data-stu-id="991ce-181">phone</span></span>               | <span data-ttu-id="991ce-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="991ce-182">String</span></span>                                | <span data-ttu-id="991ce-183">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-183">Phone number of school.</span></span>                                   |
| <span data-ttu-id="991ce-184">principalEmail</span><span class="sxs-lookup"><span data-stu-id="991ce-184">principalEmail</span></span>      | <span data-ttu-id="991ce-185">String</span><span class="sxs-lookup"><span data-stu-id="991ce-185">String</span></span>                                | <span data-ttu-id="991ce-186">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="991ce-186">Email address of the principal.</span></span>                           |
| <span data-ttu-id="991ce-187">principalName</span><span class="sxs-lookup"><span data-stu-id="991ce-187">principalName</span></span>       | <span data-ttu-id="991ce-188">String</span><span class="sxs-lookup"><span data-stu-id="991ce-188">String</span></span>                                | <span data-ttu-id="991ce-189">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="991ce-189">Name of the principal.</span></span>                                    |
| <span data-ttu-id="991ce-190">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="991ce-190">schoolNumber</span></span>        | <span data-ttu-id="991ce-191">String</span><span class="sxs-lookup"><span data-stu-id="991ce-191">String</span></span>                                | <span data-ttu-id="991ce-192">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-192">School Number.</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="991ce-193">Relações</span><span class="sxs-lookup"><span data-stu-id="991ce-193">Relationships</span></span>

| <span data-ttu-id="991ce-194">Relação</span><span class="sxs-lookup"><span data-stu-id="991ce-194">Relationship</span></span> | <span data-ttu-id="991ce-195">Tipo</span><span class="sxs-lookup"><span data-stu-id="991ce-195">Type</span></span>                                           | <span data-ttu-id="991ce-196">Descrição</span><span class="sxs-lookup"><span data-stu-id="991ce-196">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="991ce-197">classes</span><span class="sxs-lookup"><span data-stu-id="991ce-197">classes</span></span>      | <span data-ttu-id="991ce-198">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="991ce-198">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="991ce-199">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-199">Classes taught at the school.</span></span> <span data-ttu-id="991ce-200">Anulável.</span><span class="sxs-lookup"><span data-stu-id="991ce-200">Nullable.</span></span> |
| <span data-ttu-id="991ce-201">users</span><span class="sxs-lookup"><span data-stu-id="991ce-201">users</span></span>        | <span data-ttu-id="991ce-202">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="991ce-202">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="991ce-203">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="991ce-203">Users in the school.</span></span> <span data-ttu-id="991ce-204">Anulável.</span><span class="sxs-lookup"><span data-stu-id="991ce-204">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="991ce-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="991ce-205">JSON representation</span></span>

<span data-ttu-id="991ce-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="991ce-206">The following is a JSON representation of the resource.</span></span>

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
