---
title: Tipo de recurso educationSchool
description: 'Uma escola. O recurso **educationSchool** atualmente corresponde a um recurso administrativeUnit e compartilha a mesma ID.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e63fa37dacea7fee6d4378a2a6040a5cf71f3790
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37553933"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="52ae5-104">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="52ae5-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52ae5-105">Uma escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-105">A school.</span></span> <span data-ttu-id="52ae5-106">O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="52ae5-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="52ae5-107">Esse recurso é um subtipo de [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="52ae5-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="52ae5-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="52ae5-108">Methods</span></span>

| <span data-ttu-id="52ae5-109">Método</span><span class="sxs-lookup"><span data-stu-id="52ae5-109">Method</span></span>                                                                     | <span data-ttu-id="52ae5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52ae5-110">Return Type</span></span>                                      | <span data-ttu-id="52ae5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ae5-111">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="52ae5-112">Get</span><span class="sxs-lookup"><span data-stu-id="52ae5-112">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="52ae5-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="52ae5-113">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="52ae5-114">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="52ae5-114">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="52ae5-115">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="52ae5-115">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="52ae5-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="52ae5-116">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="52ae5-117">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="52ae5-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="52ae5-118">Listar classes</span><span class="sxs-lookup"><span data-stu-id="52ae5-118">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="52ae5-119">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="52ae5-119">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="52ae5-120">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="52ae5-120">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="52ae5-121">Remover classe</span><span class="sxs-lookup"><span data-stu-id="52ae5-121">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="52ae5-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="52ae5-122">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="52ae5-123">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="52ae5-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="52ae5-124">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="52ae5-124">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="52ae5-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="52ae5-125">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="52ae5-126">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="52ae5-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="52ae5-127">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="52ae5-127">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="52ae5-128">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="52ae5-128">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="52ae5-129">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="52ae5-129">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="52ae5-130">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="52ae5-130">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="52ae5-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="52ae5-131">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="52ae5-132">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="52ae5-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="52ae5-133">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="52ae5-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="52ae5-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="52ae5-134">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="52ae5-135">Obtenha o **administrativeUnit** que corresponde a esse **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="52ae5-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="52ae5-136">Atualizar</span><span class="sxs-lookup"><span data-stu-id="52ae5-136">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="52ae5-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="52ae5-137">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="52ae5-138">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="52ae5-138">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="52ae5-139">Delete</span><span class="sxs-lookup"><span data-stu-id="52ae5-139">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="52ae5-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52ae5-140">None</span></span>                                             | <span data-ttu-id="52ae5-141">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="52ae5-141">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="52ae5-142">Delta</span><span class="sxs-lookup"><span data-stu-id="52ae5-142">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="52ae5-143">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="52ae5-143">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="52ae5-144">Obter alterações incrementais para o **educationSchools**</span><span class="sxs-lookup"><span data-stu-id="52ae5-144">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="52ae5-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52ae5-145">Properties</span></span>

| <span data-ttu-id="52ae5-146">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52ae5-146">Property</span></span>            | <span data-ttu-id="52ae5-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="52ae5-147">Type</span></span>                                  | <span data-ttu-id="52ae5-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ae5-148">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="52ae5-149">id</span><span class="sxs-lookup"><span data-stu-id="52ae5-149">id</span></span>                  | <span data-ttu-id="52ae5-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-150">String</span></span>                                | <span data-ttu-id="52ae5-151">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-151">GUID of this school.</span></span>                               |
| <span data-ttu-id="52ae5-152">address</span><span class="sxs-lookup"><span data-stu-id="52ae5-152">address</span></span>             | [<span data-ttu-id="52ae5-153">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="52ae5-153">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="52ae5-154">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-154">Address of the school.</span></span>                             |
| <span data-ttu-id="52ae5-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="52ae5-155">createdBy</span></span>           | [<span data-ttu-id="52ae5-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="52ae5-156">identitySet</span></span>](identityset.md)         | <span data-ttu-id="52ae5-157">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-157">Entity who created the school.</span></span>                     |
| <span data-ttu-id="52ae5-158">description</span><span class="sxs-lookup"><span data-stu-id="52ae5-158">description</span></span>         | <span data-ttu-id="52ae5-159">String</span><span class="sxs-lookup"><span data-stu-id="52ae5-159">String</span></span>                                | <span data-ttu-id="52ae5-160">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-160">Description of the school.</span></span>                         |
| <span data-ttu-id="52ae5-161">displayName</span><span class="sxs-lookup"><span data-stu-id="52ae5-161">displayName</span></span>         | <span data-ttu-id="52ae5-162">String</span><span class="sxs-lookup"><span data-stu-id="52ae5-162">String</span></span>                                | <span data-ttu-id="52ae5-163">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-163">Display name of the school.</span></span>                        |
| <span data-ttu-id="52ae5-164">externalId</span><span class="sxs-lookup"><span data-stu-id="52ae5-164">externalId</span></span>          | <span data-ttu-id="52ae5-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-165">String</span></span>                                | <span data-ttu-id="52ae5-166">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="52ae5-166">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="52ae5-167">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="52ae5-167">externalPrincipalId</span></span> | <span data-ttu-id="52ae5-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-168">String</span></span>                                | <span data-ttu-id="52ae5-169">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="52ae5-169">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="52ae5-170">externalSource</span><span class="sxs-lookup"><span data-stu-id="52ae5-170">externalSource</span></span>      | <span data-ttu-id="52ae5-171">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-171">string</span></span>                                | <span data-ttu-id="52ae5-172">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="52ae5-172">Read-Only.</span></span> <span data-ttu-id="52ae5-173">Os valores possíveis são: `sis` ou `manual`.</span><span class="sxs-lookup"><span data-stu-id="52ae5-173">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="52ae5-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="52ae5-174">highestGrade</span></span>        | <span data-ttu-id="52ae5-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-175">String</span></span>                                | <span data-ttu-id="52ae5-176">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="52ae5-176">Highest grade taught.</span></span>                              |
| <span data-ttu-id="52ae5-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="52ae5-177">lowestGrade</span></span>         | <span data-ttu-id="52ae5-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-178">String</span></span>                                | <span data-ttu-id="52ae5-179">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="52ae5-179">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="52ae5-180">phone</span><span class="sxs-lookup"><span data-stu-id="52ae5-180">phone</span></span>               | <span data-ttu-id="52ae5-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-181">String</span></span>                                | <span data-ttu-id="52ae5-182">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-182">Phone number of school.</span></span>                            |
| <span data-ttu-id="52ae5-183">principalEmail</span><span class="sxs-lookup"><span data-stu-id="52ae5-183">principalEmail</span></span>      | <span data-ttu-id="52ae5-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-184">String</span></span>                                | <span data-ttu-id="52ae5-185">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="52ae5-185">Email address of the principal.</span></span>                    |
| <span data-ttu-id="52ae5-186">principalName</span><span class="sxs-lookup"><span data-stu-id="52ae5-186">principalName</span></span>       | <span data-ttu-id="52ae5-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-187">String</span></span>                                | <span data-ttu-id="52ae5-188">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="52ae5-188">Name of the principal.</span></span>                             |
| <span data-ttu-id="52ae5-189">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="52ae5-189">schoolNumber</span></span>        | <span data-ttu-id="52ae5-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ae5-190">String</span></span>                                | <span data-ttu-id="52ae5-191">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-191">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="52ae5-192">Relações</span><span class="sxs-lookup"><span data-stu-id="52ae5-192">Relationships</span></span>

| <span data-ttu-id="52ae5-193">Relação</span><span class="sxs-lookup"><span data-stu-id="52ae5-193">Relationship</span></span> | <span data-ttu-id="52ae5-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="52ae5-194">Type</span></span>                                           | <span data-ttu-id="52ae5-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ae5-195">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="52ae5-196">classes</span><span class="sxs-lookup"><span data-stu-id="52ae5-196">classes</span></span>      | <span data-ttu-id="52ae5-197">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="52ae5-197">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="52ae5-198">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-198">Classes taught at the school.</span></span> <span data-ttu-id="52ae5-199">Anulável.</span><span class="sxs-lookup"><span data-stu-id="52ae5-199">Nullable.</span></span> |
| <span data-ttu-id="52ae5-200">users</span><span class="sxs-lookup"><span data-stu-id="52ae5-200">users</span></span>        | <span data-ttu-id="52ae5-201">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="52ae5-201">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="52ae5-202">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="52ae5-202">Users in the school.</span></span> <span data-ttu-id="52ae5-203">Anulável.</span><span class="sxs-lookup"><span data-stu-id="52ae5-203">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="52ae5-204">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52ae5-204">JSON representation</span></span>

<span data-ttu-id="52ae5-205">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52ae5-205">The following is a JSON representation of the resource.</span></span>

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
