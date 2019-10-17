---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d7cc20b01b35f678b20e18e21dcb099a89982ab9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37553905"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="4ede3-103">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="4ede3-103">educationSchool resource type</span></span>

<span data-ttu-id="4ede3-104">Recurso usado para gerenciar aulas, professores e alunos da escola representada.</span><span class="sxs-lookup"><span data-stu-id="4ede3-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="4ede3-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4ede3-105">Methods</span></span>

| <span data-ttu-id="4ede3-106">Método</span><span class="sxs-lookup"><span data-stu-id="4ede3-106">Method</span></span>                                                   | <span data-ttu-id="4ede3-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4ede3-107">Return Type</span></span>                                    | <span data-ttu-id="4ede3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ede3-108">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="4ede3-109">Get</span><span class="sxs-lookup"><span data-stu-id="4ede3-109">Get</span></span>](../api/educationschool-get.md)                     | [<span data-ttu-id="4ede3-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="4ede3-110">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="4ede3-111">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="4ede3-111">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="4ede3-112">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="4ede3-112">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="4ede3-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="4ede3-113">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="4ede3-114">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="4ede3-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="4ede3-115">Listar classes</span><span class="sxs-lookup"><span data-stu-id="4ede3-115">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="4ede3-116">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="4ede3-116">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="4ede3-117">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="4ede3-117">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="4ede3-118">Remover classe</span><span class="sxs-lookup"><span data-stu-id="4ede3-118">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="4ede3-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="4ede3-119">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="4ede3-120">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="4ede3-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="4ede3-121">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="4ede3-121">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="4ede3-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="4ede3-122">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="4ede3-123">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="4ede3-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="4ede3-124">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="4ede3-124">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="4ede3-125">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="4ede3-125">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="4ede3-126">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="4ede3-126">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="4ede3-127">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="4ede3-127">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="4ede3-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="4ede3-128">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="4ede3-129">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="4ede3-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="4ede3-130">Atualizar</span><span class="sxs-lookup"><span data-stu-id="4ede3-130">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="4ede3-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="4ede3-131">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="4ede3-132">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="4ede3-132">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="4ede3-133">Delete</span><span class="sxs-lookup"><span data-stu-id="4ede3-133">Delete</span></span>](../api/educationschool-delete.md)               | <span data-ttu-id="4ede3-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ede3-134">None</span></span>                                           | <span data-ttu-id="4ede3-135">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="4ede3-135">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="4ede3-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ede3-136">Properties</span></span>

| <span data-ttu-id="4ede3-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ede3-137">Property</span></span>            | <span data-ttu-id="4ede3-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ede3-138">Type</span></span>                                  | <span data-ttu-id="4ede3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ede3-139">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="4ede3-140">id</span><span class="sxs-lookup"><span data-stu-id="4ede3-140">id</span></span>                  | <span data-ttu-id="4ede3-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-141">String</span></span>                                | <span data-ttu-id="4ede3-142">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="4ede3-142">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="4ede3-143">displayName</span><span class="sxs-lookup"><span data-stu-id="4ede3-143">displayName</span></span>         | <span data-ttu-id="4ede3-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-144">String</span></span>                                | <span data-ttu-id="4ede3-145">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="4ede3-145">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="4ede3-146">description</span><span class="sxs-lookup"><span data-stu-id="4ede3-146">description</span></span>         | <span data-ttu-id="4ede3-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-147">String</span></span>                                | <span data-ttu-id="4ede3-148">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="4ede3-148">Description of the school.</span></span>                                                         |
| <span data-ttu-id="4ede3-149">status</span><span class="sxs-lookup"><span data-stu-id="4ede3-149">status</span></span>              | <span data-ttu-id="4ede3-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-150">string</span></span>                                | <span data-ttu-id="4ede3-151">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="4ede3-151">Read-Only.</span></span> <span data-ttu-id="4ede3-152">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="4ede3-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="4ede3-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="4ede3-153">externalSource</span></span>      | <span data-ttu-id="4ede3-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="4ede3-154">educationExternalSource</span></span>               | <span data-ttu-id="4ede3-155">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="4ede3-155">Read-Only.</span></span>  <span data-ttu-id="4ede3-156">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4ede3-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="4ede3-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="4ede3-157">principalEmail</span></span>      | <span data-ttu-id="4ede3-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-158">String</span></span>                                | <span data-ttu-id="4ede3-159">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="4ede3-159">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="4ede3-160">principalName</span><span class="sxs-lookup"><span data-stu-id="4ede3-160">principalName</span></span>       | <span data-ttu-id="4ede3-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-161">String</span></span>                                | <span data-ttu-id="4ede3-162">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="4ede3-162">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="4ede3-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="4ede3-163">externalPrincipalId</span></span> | <span data-ttu-id="4ede3-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-164">String</span></span>                                | <span data-ttu-id="4ede3-165">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4ede3-165">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="4ede3-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="4ede3-166">highestGrade</span></span>        | <span data-ttu-id="4ede3-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-167">String</span></span>                                | <span data-ttu-id="4ede3-168">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="4ede3-168">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="4ede3-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="4ede3-169">lowestGrade</span></span>         | <span data-ttu-id="4ede3-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-170">String</span></span>                                | <span data-ttu-id="4ede3-171">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="4ede3-171">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="4ede3-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="4ede3-172">schoolNumber</span></span>        | <span data-ttu-id="4ede3-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-173">String</span></span>                                | <span data-ttu-id="4ede3-174">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="4ede3-174">School Number.</span></span>                                                                     |
| <span data-ttu-id="4ede3-175">externalId</span><span class="sxs-lookup"><span data-stu-id="4ede3-175">externalId</span></span>          | <span data-ttu-id="4ede3-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-176">String</span></span>                                | <span data-ttu-id="4ede3-177">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4ede3-177">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="4ede3-178">phone</span><span class="sxs-lookup"><span data-stu-id="4ede3-178">phone</span></span>               | <span data-ttu-id="4ede3-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ede3-179">String</span></span>                                | <span data-ttu-id="4ede3-180">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="4ede3-180">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="4ede3-181">address</span><span class="sxs-lookup"><span data-stu-id="4ede3-181">address</span></span>             | [<span data-ttu-id="4ede3-182">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4ede3-182">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="4ede3-183">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="4ede3-183">Address of the school.</span></span>                                                             |
| <span data-ttu-id="4ede3-184">createdBy</span><span class="sxs-lookup"><span data-stu-id="4ede3-184">createdBy</span></span>           | [<span data-ttu-id="4ede3-185">identitySet</span><span class="sxs-lookup"><span data-stu-id="4ede3-185">identitySet</span></span>](identityset.md)         | <span data-ttu-id="4ede3-186">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="4ede3-186">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="4ede3-187">Relações</span><span class="sxs-lookup"><span data-stu-id="4ede3-187">Relationships</span></span>

| <span data-ttu-id="4ede3-188">Relação</span><span class="sxs-lookup"><span data-stu-id="4ede3-188">Relationship</span></span> | <span data-ttu-id="4ede3-189">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ede3-189">Type</span></span>                                           | <span data-ttu-id="4ede3-190">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ede3-190">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="4ede3-191">classes</span><span class="sxs-lookup"><span data-stu-id="4ede3-191">classes</span></span>      | <span data-ttu-id="4ede3-192">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="4ede3-192">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="4ede3-193">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="4ede3-193">Classes taught at the school.</span></span> <span data-ttu-id="4ede3-194">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4ede3-194">Nullable.</span></span> |
| <span data-ttu-id="4ede3-195">users</span><span class="sxs-lookup"><span data-stu-id="4ede3-195">users</span></span>        | <span data-ttu-id="4ede3-196">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="4ede3-196">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="4ede3-197">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="4ede3-197">Users in the school.</span></span> <span data-ttu-id="4ede3-198">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4ede3-198">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="4ede3-199">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ede3-199">JSON representation</span></span>

<span data-ttu-id="4ede3-200">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ede3-200">The following is a JSON representation of the resource.</span></span>

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
