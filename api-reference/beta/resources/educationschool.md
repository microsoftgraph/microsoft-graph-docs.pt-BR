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
# <a name="educationschool-resource-type"></a><span data-ttu-id="8da68-104">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="8da68-104">educationSchool resource type</span></span>

<span data-ttu-id="8da68-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8da68-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8da68-106">Uma escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-106">A school.</span></span> <span data-ttu-id="8da68-107">O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="8da68-107">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="8da68-108">Esse recurso é um subtipo de [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="8da68-108">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8da68-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="8da68-109">Methods</span></span>

| <span data-ttu-id="8da68-110">Método</span><span class="sxs-lookup"><span data-stu-id="8da68-110">Method</span></span>                                                                     | <span data-ttu-id="8da68-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8da68-111">Return Type</span></span>                                      | <span data-ttu-id="8da68-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8da68-112">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="8da68-113">Get</span><span class="sxs-lookup"><span data-stu-id="8da68-113">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="8da68-114">educationSchool</span><span class="sxs-lookup"><span data-stu-id="8da68-114">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="8da68-115">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="8da68-115">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="8da68-116">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="8da68-116">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="8da68-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="8da68-117">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="8da68-118">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="8da68-118">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="8da68-119">Listar classes</span><span class="sxs-lookup"><span data-stu-id="8da68-119">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="8da68-120">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="8da68-120">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="8da68-121">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="8da68-121">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="8da68-122">Remover classe</span><span class="sxs-lookup"><span data-stu-id="8da68-122">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="8da68-123">educationClass</span><span class="sxs-lookup"><span data-stu-id="8da68-123">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="8da68-124">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="8da68-124">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="8da68-125">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="8da68-125">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="8da68-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="8da68-126">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="8da68-127">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="8da68-127">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="8da68-128">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="8da68-128">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="8da68-129">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="8da68-129">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="8da68-130">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="8da68-130">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="8da68-131">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="8da68-131">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="8da68-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="8da68-132">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="8da68-133">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="8da68-133">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="8da68-134">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="8da68-134">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="8da68-135">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="8da68-135">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="8da68-136">Obtenha o **administrativeUnit** que corresponde a esse **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="8da68-136">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="8da68-137">Atualizar</span><span class="sxs-lookup"><span data-stu-id="8da68-137">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="8da68-138">educationSchool</span><span class="sxs-lookup"><span data-stu-id="8da68-138">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="8da68-139">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="8da68-139">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="8da68-140">Delete</span><span class="sxs-lookup"><span data-stu-id="8da68-140">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="8da68-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8da68-141">None</span></span>                                             | <span data-ttu-id="8da68-142">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="8da68-142">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="8da68-143">Delta</span><span class="sxs-lookup"><span data-stu-id="8da68-143">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="8da68-144">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="8da68-144">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="8da68-145">Obter alterações incrementais para o **educationSchools**</span><span class="sxs-lookup"><span data-stu-id="8da68-145">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="8da68-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8da68-146">Properties</span></span>

| <span data-ttu-id="8da68-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8da68-147">Property</span></span>            | <span data-ttu-id="8da68-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="8da68-148">Type</span></span>                                  | <span data-ttu-id="8da68-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="8da68-149">Description</span></span>                                               |
| :------------------ | :------------------------------------ | :-------------------------------------------------------- |
| <span data-ttu-id="8da68-150">id</span><span class="sxs-lookup"><span data-stu-id="8da68-150">id</span></span>                  | <span data-ttu-id="8da68-151">String</span><span class="sxs-lookup"><span data-stu-id="8da68-151">String</span></span>                                | <span data-ttu-id="8da68-152">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-152">GUID of this school.</span></span>                                      |
| <span data-ttu-id="8da68-153">address</span><span class="sxs-lookup"><span data-stu-id="8da68-153">address</span></span>             | [<span data-ttu-id="8da68-154">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="8da68-154">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="8da68-155">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-155">Address of the school.</span></span>                                    |
| <span data-ttu-id="8da68-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="8da68-156">createdBy</span></span>           | [<span data-ttu-id="8da68-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="8da68-157">identitySet</span></span>](identityset.md)         | <span data-ttu-id="8da68-158">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-158">Entity who created the school.</span></span>                            |
| <span data-ttu-id="8da68-159">description</span><span class="sxs-lookup"><span data-stu-id="8da68-159">description</span></span>         | <span data-ttu-id="8da68-160">String</span><span class="sxs-lookup"><span data-stu-id="8da68-160">String</span></span>                                | <span data-ttu-id="8da68-161">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-161">Description of the school.</span></span>                                |
| <span data-ttu-id="8da68-162">displayName</span><span class="sxs-lookup"><span data-stu-id="8da68-162">displayName</span></span>         | <span data-ttu-id="8da68-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8da68-163">String</span></span>                                | <span data-ttu-id="8da68-164">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-164">Display name of the school.</span></span>                               |
| <span data-ttu-id="8da68-165">externalId</span><span class="sxs-lookup"><span data-stu-id="8da68-165">externalId</span></span>          | <span data-ttu-id="8da68-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8da68-166">String</span></span>                                | <span data-ttu-id="8da68-167">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8da68-167">ID of school in syncing system.</span></span>                           |
| <span data-ttu-id="8da68-168">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="8da68-168">externalPrincipalId</span></span> | <span data-ttu-id="8da68-169">String</span><span class="sxs-lookup"><span data-stu-id="8da68-169">String</span></span>                                | <span data-ttu-id="8da68-170">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8da68-170">ID of principal in syncing system.</span></span>                        |
| <span data-ttu-id="8da68-171">externalSource</span><span class="sxs-lookup"><span data-stu-id="8da68-171">externalSource</span></span>      | <span data-ttu-id="8da68-172">String</span><span class="sxs-lookup"><span data-stu-id="8da68-172">String</span></span>                                | <span data-ttu-id="8da68-173">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="8da68-173">Read-Only.</span></span> <span data-ttu-id="8da68-174">Os valores possíveis são: `sis` , `lms` ou `manual` .</span><span class="sxs-lookup"><span data-stu-id="8da68-174">Possible values are: `sis`, `lms` or `manual`.</span></span> |
| <span data-ttu-id="8da68-175">highestGrade</span><span class="sxs-lookup"><span data-stu-id="8da68-175">highestGrade</span></span>        | <span data-ttu-id="8da68-176">String</span><span class="sxs-lookup"><span data-stu-id="8da68-176">String</span></span>                                | <span data-ttu-id="8da68-177">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="8da68-177">Highest grade taught.</span></span>                                     |
| <span data-ttu-id="8da68-178">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="8da68-178">lowestGrade</span></span>         | <span data-ttu-id="8da68-179">String</span><span class="sxs-lookup"><span data-stu-id="8da68-179">String</span></span>                                | <span data-ttu-id="8da68-180">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="8da68-180">Lowest grade taught.</span></span>                                      |
| <span data-ttu-id="8da68-181">phone</span><span class="sxs-lookup"><span data-stu-id="8da68-181">phone</span></span>               | <span data-ttu-id="8da68-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8da68-182">String</span></span>                                | <span data-ttu-id="8da68-183">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-183">Phone number of school.</span></span>                                   |
| <span data-ttu-id="8da68-184">principalEmail</span><span class="sxs-lookup"><span data-stu-id="8da68-184">principalEmail</span></span>      | <span data-ttu-id="8da68-185">String</span><span class="sxs-lookup"><span data-stu-id="8da68-185">String</span></span>                                | <span data-ttu-id="8da68-186">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="8da68-186">Email address of the principal.</span></span>                           |
| <span data-ttu-id="8da68-187">principalName</span><span class="sxs-lookup"><span data-stu-id="8da68-187">principalName</span></span>       | <span data-ttu-id="8da68-188">String</span><span class="sxs-lookup"><span data-stu-id="8da68-188">String</span></span>                                | <span data-ttu-id="8da68-189">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="8da68-189">Name of the principal.</span></span>                                    |
| <span data-ttu-id="8da68-190">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="8da68-190">schoolNumber</span></span>        | <span data-ttu-id="8da68-191">String</span><span class="sxs-lookup"><span data-stu-id="8da68-191">String</span></span>                                | <span data-ttu-id="8da68-192">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-192">School Number.</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="8da68-193">Relações</span><span class="sxs-lookup"><span data-stu-id="8da68-193">Relationships</span></span>

| <span data-ttu-id="8da68-194">Relação</span><span class="sxs-lookup"><span data-stu-id="8da68-194">Relationship</span></span> | <span data-ttu-id="8da68-195">Tipo</span><span class="sxs-lookup"><span data-stu-id="8da68-195">Type</span></span>                                           | <span data-ttu-id="8da68-196">Descrição</span><span class="sxs-lookup"><span data-stu-id="8da68-196">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="8da68-197">classes</span><span class="sxs-lookup"><span data-stu-id="8da68-197">classes</span></span>      | <span data-ttu-id="8da68-198">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="8da68-198">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="8da68-199">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-199">Classes taught at the school.</span></span> <span data-ttu-id="8da68-200">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8da68-200">Nullable.</span></span> |
| <span data-ttu-id="8da68-201">users</span><span class="sxs-lookup"><span data-stu-id="8da68-201">users</span></span>        | <span data-ttu-id="8da68-202">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="8da68-202">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="8da68-203">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="8da68-203">Users in the school.</span></span> <span data-ttu-id="8da68-204">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8da68-204">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="8da68-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8da68-205">JSON representation</span></span>

<span data-ttu-id="8da68-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8da68-206">The following is a JSON representation of the resource.</span></span>

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
