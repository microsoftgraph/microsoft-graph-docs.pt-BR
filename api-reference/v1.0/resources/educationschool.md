---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 407f29c7d8f9468c5e9b1da1badad294cb655121
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531513"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="cfbdc-103">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="cfbdc-103">educationSchool resource type</span></span>

<span data-ttu-id="cfbdc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfbdc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cfbdc-105">Recurso usado para gerenciar aulas, professores e alunos da escola representada.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-105">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="cfbdc-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cfbdc-106">Methods</span></span>

| <span data-ttu-id="cfbdc-107">Método</span><span class="sxs-lookup"><span data-stu-id="cfbdc-107">Method</span></span>                                                   | <span data-ttu-id="cfbdc-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cfbdc-108">Return Type</span></span>                                    | <span data-ttu-id="cfbdc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfbdc-109">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="cfbdc-110">Get</span><span class="sxs-lookup"><span data-stu-id="cfbdc-110">Get</span></span>](../api/educationschool-get.md)                     | [<span data-ttu-id="cfbdc-111">educationSchool</span><span class="sxs-lookup"><span data-stu-id="cfbdc-111">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="cfbdc-112">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-112">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="cfbdc-113">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="cfbdc-113">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="cfbdc-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="cfbdc-114">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="cfbdc-115">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-115">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="cfbdc-116">Listar classes</span><span class="sxs-lookup"><span data-stu-id="cfbdc-116">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="cfbdc-117">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="cfbdc-117">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="cfbdc-118">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-118">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="cfbdc-119">Remover classe</span><span class="sxs-lookup"><span data-stu-id="cfbdc-119">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="cfbdc-120">educationClass</span><span class="sxs-lookup"><span data-stu-id="cfbdc-120">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="cfbdc-121">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-121">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="cfbdc-122">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="cfbdc-122">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="cfbdc-123">educationUser</span><span class="sxs-lookup"><span data-stu-id="cfbdc-123">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="cfbdc-124">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-124">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="cfbdc-125">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="cfbdc-125">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="cfbdc-126">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="cfbdc-126">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="cfbdc-127">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-127">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="cfbdc-128">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="cfbdc-128">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="cfbdc-129">educationUser</span><span class="sxs-lookup"><span data-stu-id="cfbdc-129">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="cfbdc-130">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-130">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="cfbdc-131">Atualizar</span><span class="sxs-lookup"><span data-stu-id="cfbdc-131">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="cfbdc-132">educationSchool</span><span class="sxs-lookup"><span data-stu-id="cfbdc-132">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="cfbdc-133">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-133">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="cfbdc-134">Excluir</span><span class="sxs-lookup"><span data-stu-id="cfbdc-134">Delete</span></span>](../api/educationschool-delete.md)               | <span data-ttu-id="cfbdc-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cfbdc-135">None</span></span>                                           | <span data-ttu-id="cfbdc-136">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-136">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="cfbdc-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfbdc-137">Properties</span></span>

| <span data-ttu-id="cfbdc-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfbdc-138">Property</span></span>            | <span data-ttu-id="cfbdc-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfbdc-139">Type</span></span>                                  | <span data-ttu-id="cfbdc-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfbdc-140">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="cfbdc-141">id</span><span class="sxs-lookup"><span data-stu-id="cfbdc-141">id</span></span>                  | <span data-ttu-id="cfbdc-142">String</span><span class="sxs-lookup"><span data-stu-id="cfbdc-142">String</span></span>                                | <span data-ttu-id="cfbdc-143">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-143">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="cfbdc-144">displayName</span><span class="sxs-lookup"><span data-stu-id="cfbdc-144">displayName</span></span>         | <span data-ttu-id="cfbdc-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfbdc-145">String</span></span>                                | <span data-ttu-id="cfbdc-146">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-146">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="cfbdc-147">description</span><span class="sxs-lookup"><span data-stu-id="cfbdc-147">description</span></span>         | <span data-ttu-id="cfbdc-148">String</span><span class="sxs-lookup"><span data-stu-id="cfbdc-148">String</span></span>                                | <span data-ttu-id="cfbdc-149">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-149">Description of the school.</span></span>                                                         |
| <span data-ttu-id="cfbdc-150">status</span><span class="sxs-lookup"><span data-stu-id="cfbdc-150">status</span></span>              | <span data-ttu-id="cfbdc-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfbdc-151">string</span></span>                                | <span data-ttu-id="cfbdc-152">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-152">Read-Only.</span></span> <span data-ttu-id="cfbdc-153">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-153">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="cfbdc-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="cfbdc-154">externalSource</span></span>      | <span data-ttu-id="cfbdc-155">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="cfbdc-155">educationExternalSource</span></span>               | <span data-ttu-id="cfbdc-156">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-156">Read-Only.</span></span>  <span data-ttu-id="cfbdc-157">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-157">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="cfbdc-158">principalEmail</span><span class="sxs-lookup"><span data-stu-id="cfbdc-158">principalEmail</span></span>      | <span data-ttu-id="cfbdc-159">String</span><span class="sxs-lookup"><span data-stu-id="cfbdc-159">String</span></span>                                | <span data-ttu-id="cfbdc-160">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-160">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="cfbdc-161">principalName</span><span class="sxs-lookup"><span data-stu-id="cfbdc-161">principalName</span></span>       | <span data-ttu-id="cfbdc-162">String</span><span class="sxs-lookup"><span data-stu-id="cfbdc-162">String</span></span>                                | <span data-ttu-id="cfbdc-163">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-163">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="cfbdc-164">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="cfbdc-164">externalPrincipalId</span></span> | <span data-ttu-id="cfbdc-165">String</span><span class="sxs-lookup"><span data-stu-id="cfbdc-165">String</span></span>                                | <span data-ttu-id="cfbdc-166">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-166">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="cfbdc-167">highestGrade</span><span class="sxs-lookup"><span data-stu-id="cfbdc-167">highestGrade</span></span>        | <span data-ttu-id="cfbdc-168">String</span><span class="sxs-lookup"><span data-stu-id="cfbdc-168">String</span></span>                                | <span data-ttu-id="cfbdc-169">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-169">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="cfbdc-170">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="cfbdc-170">lowestGrade</span></span>         | <span data-ttu-id="cfbdc-171">String</span><span class="sxs-lookup"><span data-stu-id="cfbdc-171">String</span></span>                                | <span data-ttu-id="cfbdc-172">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-172">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="cfbdc-173">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="cfbdc-173">schoolNumber</span></span>        | <span data-ttu-id="cfbdc-174">String</span><span class="sxs-lookup"><span data-stu-id="cfbdc-174">String</span></span>                                | <span data-ttu-id="cfbdc-175">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-175">School Number.</span></span>                                                                     |
| <span data-ttu-id="cfbdc-176">externalId</span><span class="sxs-lookup"><span data-stu-id="cfbdc-176">externalId</span></span>          | <span data-ttu-id="cfbdc-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfbdc-177">String</span></span>                                | <span data-ttu-id="cfbdc-178">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-178">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="cfbdc-179">phone</span><span class="sxs-lookup"><span data-stu-id="cfbdc-179">phone</span></span>               | <span data-ttu-id="cfbdc-180">String</span><span class="sxs-lookup"><span data-stu-id="cfbdc-180">String</span></span>                                | <span data-ttu-id="cfbdc-181">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-181">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="cfbdc-182">address</span><span class="sxs-lookup"><span data-stu-id="cfbdc-182">address</span></span>             | [<span data-ttu-id="cfbdc-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="cfbdc-183">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="cfbdc-184">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-184">Address of the school.</span></span>                                                             |
| <span data-ttu-id="cfbdc-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="cfbdc-185">createdBy</span></span>           | [<span data-ttu-id="cfbdc-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="cfbdc-186">identitySet</span></span>](identityset.md)         | <span data-ttu-id="cfbdc-187">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-187">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="cfbdc-188">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="cfbdc-188">Relationships</span></span>

| <span data-ttu-id="cfbdc-189">Relação</span><span class="sxs-lookup"><span data-stu-id="cfbdc-189">Relationship</span></span> | <span data-ttu-id="cfbdc-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfbdc-190">Type</span></span>                                           | <span data-ttu-id="cfbdc-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfbdc-191">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="cfbdc-192">classes</span><span class="sxs-lookup"><span data-stu-id="cfbdc-192">classes</span></span>      | <span data-ttu-id="cfbdc-193">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="cfbdc-193">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="cfbdc-194">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-194">Classes taught at the school.</span></span> <span data-ttu-id="cfbdc-195">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-195">Nullable.</span></span> |
| <span data-ttu-id="cfbdc-196">users</span><span class="sxs-lookup"><span data-stu-id="cfbdc-196">users</span></span>        | <span data-ttu-id="cfbdc-197">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="cfbdc-197">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="cfbdc-198">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-198">Users in the school.</span></span> <span data-ttu-id="cfbdc-199">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-199">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="cfbdc-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfbdc-200">JSON representation</span></span>

<span data-ttu-id="cfbdc-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfbdc-201">The following is a JSON representation of the resource.</span></span>

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
