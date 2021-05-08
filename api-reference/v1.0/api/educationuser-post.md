---
title: Criar educationUser
description: Crie um novo objeto educationUser.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b26e0530fd4beea6d2f604fa46f891e154fefa61
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232144"
---
# <a name="create-educationuser"></a><span data-ttu-id="13047-103">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="13047-103">Create educationUser</span></span>

<span data-ttu-id="13047-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13047-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13047-105">Crie um novo [objeto educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="13047-105">Create a new [educationUser](../resources/educationuser.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="13047-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="13047-106">Permissions</span></span>

<span data-ttu-id="13047-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13047-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13047-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13047-109">Permission type</span></span>                        | <span data-ttu-id="13047-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13047-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="13047-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13047-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="13047-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13047-112">Not supported.</span></span>                              |
| <span data-ttu-id="13047-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13047-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13047-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13047-114">Not supported.</span></span>                              |
| <span data-ttu-id="13047-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13047-115">Application</span></span>                            | <span data-ttu-id="13047-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13047-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="13047-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13047-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/users
```

## <a name="request-headers"></a><span data-ttu-id="13047-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13047-118">Request headers</span></span>

| <span data-ttu-id="13047-119">Nome</span><span class="sxs-lookup"><span data-stu-id="13047-119">Name</span></span>          | <span data-ttu-id="13047-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="13047-120">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="13047-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="13047-121">Authorization</span></span> | <span data-ttu-id="13047-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13047-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="13047-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13047-124">Content-Type</span></span>  | <span data-ttu-id="13047-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13047-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13047-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13047-127">Request body</span></span>

<span data-ttu-id="13047-128">No corpo da solicitação, fornece uma representação JSON do [objeto educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="13047-128">In the request body, supply a JSON representation of the [educationUser](../resources/educationuser.md) object.</span></span>

<span data-ttu-id="13047-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="13047-129">The following table shows the properties that are required when you create the [educationUser](../resources/educationuser.md).</span></span>

| <span data-ttu-id="13047-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13047-130">Property</span></span>             | <span data-ttu-id="13047-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13047-131">Type</span></span>                                                               | <span data-ttu-id="13047-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13047-132">Description</span></span>                                                                                                                                                                                                                                                                                                                                                 |
| :------------------- | :----------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="13047-133">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="13047-133">accountEnabled</span></span>       | <span data-ttu-id="13047-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="13047-134">Boolean</span></span>                                                            | <span data-ttu-id="13047-135">**True** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="13047-135">**True** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="13047-136">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="13047-136">This property is required when a user is created.</span></span> <span data-ttu-id="13047-137">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="13047-137">Supports $filter.</span></span>                                                                                                                                                                                                                               |
| <span data-ttu-id="13047-138">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="13047-138">assignedLicenses</span></span>     | <span data-ttu-id="13047-139">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="13047-139">[assignedLicense](../resources/assignedlicense.md) collection</span></span>      | <span data-ttu-id="13047-p105">As licenças que são atribuídas ao usuário. Não anulável.</span><span class="sxs-lookup"><span data-stu-id="13047-p105">The licenses that are assigned to the user. Not nullable.</span></span>                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="13047-142">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="13047-142">assignedPlans</span></span>        | <span data-ttu-id="13047-143">Coleção [assignedPlan](../resources/assignedplan.md)</span><span class="sxs-lookup"><span data-stu-id="13047-143">[assignedPlan](../resources/assignedplan.md) collection</span></span>            | <span data-ttu-id="13047-p106">Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.</span><span class="sxs-lookup"><span data-stu-id="13047-p106">The plans that are assigned to the user. Read-only. Not nullable.</span></span>                                                                                                                                                                                                                                                                                           |
| <span data-ttu-id="13047-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="13047-147">businessPhones</span></span>       | <span data-ttu-id="13047-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="13047-148">String collection</span></span>                                                  | <span data-ttu-id="13047-149">Números de telefone para o usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-149">The telephone numbers for the user.</span></span> <span data-ttu-id="13047-150">**Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="13047-150">**Note:** Although this is a string collection, only one number can be set for this property.</span></span>                                                                                                                                                                                                                           |
| <span data-ttu-id="13047-151">createdBy</span><span class="sxs-lookup"><span data-stu-id="13047-151">createdBy</span></span>            | [<span data-ttu-id="13047-152">identitySet</span><span class="sxs-lookup"><span data-stu-id="13047-152">identitySet</span></span>](../resources/identityset.md)                         | <span data-ttu-id="13047-153">Entidade que criou o usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-153">Entity who created the user.</span></span>                                                                                                                                                                                                                                                                                                                                |
| <span data-ttu-id="13047-154">department</span><span class="sxs-lookup"><span data-stu-id="13047-154">department</span></span>           | <span data-ttu-id="13047-155">String</span><span class="sxs-lookup"><span data-stu-id="13047-155">String</span></span>                                                             | <span data-ttu-id="13047-p108">O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="13047-p108">The name for the department in which the user works. Supports $filter.</span></span>                                                                                                                                                                                                                                                                                      |
| <span data-ttu-id="13047-158">displayName</span><span class="sxs-lookup"><span data-stu-id="13047-158">displayName</span></span>          | <span data-ttu-id="13047-159">String</span><span class="sxs-lookup"><span data-stu-id="13047-159">String</span></span>                                                             | <span data-ttu-id="13047-160">O nome exibido para o usuário no catálogo de endereços.</span><span class="sxs-lookup"><span data-stu-id="13047-160">The name displayed in the address book for the user.</span></span> <span data-ttu-id="13047-161">Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-161">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="13047-162">Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="13047-162">This property is required when a user is created and it cannot be cleared during updates.</span></span> <span data-ttu-id="13047-163">Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="13047-163">Supports $filter and $orderby.</span></span>                                                                                      |
| <span data-ttu-id="13047-164">externalSource</span><span class="sxs-lookup"><span data-stu-id="13047-164">externalSource</span></span>       | <span data-ttu-id="13047-165">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="13047-165">educationExternalSource</span></span>                                            | <span data-ttu-id="13047-166">De onde esse usuário foi criado.</span><span class="sxs-lookup"><span data-stu-id="13047-166">Where this user was created from.</span></span> <span data-ttu-id="13047-167">Os valores possíveis são: `sis` e `manual`.</span><span class="sxs-lookup"><span data-stu-id="13047-167">Possible values are: `sis`, `manual`.</span></span>                                                                                                                                                                                                                                                                                     |
| <span data-ttu-id="13047-168">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="13047-168">externalSourceDetail</span></span> | <span data-ttu-id="13047-169">String</span><span class="sxs-lookup"><span data-stu-id="13047-169">String</span></span>                                                             | <span data-ttu-id="13047-170">O nome da fonte externa de onde esses recursos foram gerados.</span><span class="sxs-lookup"><span data-stu-id="13047-170">The name of the external source this resources was generated from.</span></span>                                                                                                                                                                                                                                                                                          |
| <span data-ttu-id="13047-171">givenName</span><span class="sxs-lookup"><span data-stu-id="13047-171">givenName</span></span>            | <span data-ttu-id="13047-172">String</span><span class="sxs-lookup"><span data-stu-id="13047-172">String</span></span>                                                             | <span data-ttu-id="13047-p111">O nome fornecido (nome) do usuário. Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="13047-p111">The given name (first name) of the user. Supports $filter.</span></span>                                                                                                                                                                                                                                                                                                  |
| <span data-ttu-id="13047-175">email</span><span class="sxs-lookup"><span data-stu-id="13047-175">mail</span></span>                 | <span data-ttu-id="13047-176">String</span><span class="sxs-lookup"><span data-stu-id="13047-176">String</span></span>                                                             | <span data-ttu-id="13047-177">O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com".</span><span class="sxs-lookup"><span data-stu-id="13047-177">The SMTP address for the user; for example, "jeff@contoso.onmicrosoft.com".</span></span> <span data-ttu-id="13047-178">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="13047-178">Read-Only.</span></span> <span data-ttu-id="13047-179">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="13047-179">Supports $filter.</span></span>                                                                                                                                                                                                                                                    |
| <span data-ttu-id="13047-180">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="13047-180">mailingAddress</span></span>       | [<span data-ttu-id="13047-181">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="13047-181">physicalAddress</span></span>](../resources/physicaladdress.md)                 | <span data-ttu-id="13047-182">Endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-182">Mail address of user.</span></span>                                                                                                                                                                                                                                                                                                                                       |
| <span data-ttu-id="13047-183">mailNickname</span><span class="sxs-lookup"><span data-stu-id="13047-183">mailNickname</span></span>         | <span data-ttu-id="13047-184">String</span><span class="sxs-lookup"><span data-stu-id="13047-184">String</span></span>                                                             | <span data-ttu-id="13047-p113">O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="13047-p113">The mail alias for the user. This property must be specified when a user is created. Supports $filter.</span></span>                                                                                                                                                                                                                                                      |
| <span data-ttu-id="13047-188">middleName</span><span class="sxs-lookup"><span data-stu-id="13047-188">middleName</span></span>           | <span data-ttu-id="13047-189">String</span><span class="sxs-lookup"><span data-stu-id="13047-189">String</span></span>                                                             | <span data-ttu-id="13047-190">O nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-190">The middle name of user.</span></span>                                                                                                                                                                                                                                                                                                                                    |
| <span data-ttu-id="13047-191">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="13047-191">mobilePhone</span></span>          | <span data-ttu-id="13047-192">String</span><span class="sxs-lookup"><span data-stu-id="13047-192">String</span></span>                                                             | <span data-ttu-id="13047-193">O número de celular principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-193">The primary cellular telephone number for the user.</span></span>                                                                                                                                                                                                                                                                                                         |
| <span data-ttu-id="13047-194">onPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="13047-194">onPremisesInfo</span></span>       | [<span data-ttu-id="13047-195">educationOnPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="13047-195">educationOnPremisesInfo</span></span>](../resources/educationonpremisesinfo.md) | <span data-ttu-id="13047-196">Informações adicionais usadas para associar o usuário do AAD ao equivalente do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="13047-196">Additional information used to associate the AAD user with it's Active Directory counterpart.</span></span>                                                                                                                                                                                                                                                               |
| <span data-ttu-id="13047-197">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="13047-197">passwordPolicies</span></span>     | <span data-ttu-id="13047-198">String</span><span class="sxs-lookup"><span data-stu-id="13047-198">String</span></span>                                                             | <span data-ttu-id="13047-199">Especifica as políticas de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-199">Specifies password policies for the user.</span></span> <span data-ttu-id="13047-200">Este valor é uma enumeração com um possível valor sendo "DisableStrongPassword", que permite especificar as senhas mais fracas do que a política padrão.</span><span class="sxs-lookup"><span data-stu-id="13047-200">This value is an enumeration with one possible value being "DisableStrongPassword", which allows weaker passwords than the default policy to be specified.</span></span> <span data-ttu-id="13047-201">O "DisablePasswordExpiration" também pode ser especificado.</span><span class="sxs-lookup"><span data-stu-id="13047-201">"DisablePasswordExpiration" can also be specified.</span></span> <span data-ttu-id="13047-202">Os dois podem ser especificados juntos, por exemplo: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="13047-202">The two can be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span> |
| <span data-ttu-id="13047-203">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="13047-203">passwordProfile</span></span>      | [<span data-ttu-id="13047-204">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="13047-204">passwordProfile</span></span>](../resources/passwordprofile.md)                 | <span data-ttu-id="13047-205">Especifica o perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-205">Specifies the password profile for the user.</span></span> <span data-ttu-id="13047-206">O perfil contém a senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-206">The profile contains the user's password.</span></span> <span data-ttu-id="13047-207">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="13047-207">This property is required when a user is created.</span></span> <span data-ttu-id="13047-208">A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**.</span><span class="sxs-lookup"><span data-stu-id="13047-208">The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property.</span></span> <span data-ttu-id="13047-209">Por padrão, é obrigatória uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="13047-209">By default, a strong password is required.</span></span>                                                        |
| <span data-ttu-id="13047-210">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="13047-210">preferredLanguage</span></span>    | <span data-ttu-id="13047-211">String</span><span class="sxs-lookup"><span data-stu-id="13047-211">String</span></span>                                                             | <span data-ttu-id="13047-212">O idioma preferencial do usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-212">The preferred language for the user.</span></span> <span data-ttu-id="13047-213">Deve seguir o código ISO 639-1; por exemplo, "en-US".</span><span class="sxs-lookup"><span data-stu-id="13047-213">Should follow ISO 639-1 Code; for example, "en-US".</span></span>                                                                                                                                                                                                                                                                    |
| <span data-ttu-id="13047-214">primaryRole</span><span class="sxs-lookup"><span data-stu-id="13047-214">primaryRole</span></span>          | <span data-ttu-id="13047-215">educationUserRole</span><span class="sxs-lookup"><span data-stu-id="13047-215">educationUserRole</span></span>                                                  | <span data-ttu-id="13047-216">Função padrão de um usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-216">Default role for a user.</span></span> <span data-ttu-id="13047-217">A função do usuário pode ser diferente em uma aula individual.</span><span class="sxs-lookup"><span data-stu-id="13047-217">The user's role might be different in an individual class.</span></span> <span data-ttu-id="13047-218">Os valores possíveis são: `student`, `teacher`, `none`.</span><span class="sxs-lookup"><span data-stu-id="13047-218">Possible values are: `student`, `teacher`, `none`.</span></span>                                                                                                                                                                                                                      |
| <span data-ttu-id="13047-219">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="13047-219">provisionedPlans</span></span>     | <span data-ttu-id="13047-220">coleção [provisionedPlan](../resources/provisionedplan.md)</span><span class="sxs-lookup"><span data-stu-id="13047-220">[provisionedPlan](../resources/provisionedplan.md) collection</span></span>      | <span data-ttu-id="13047-p118">Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.</span><span class="sxs-lookup"><span data-stu-id="13047-p118">The plans that are provisioned for the user. Read-only. Not nullable.</span></span>                                                                                                                                                                                                                                                                                       |
| <span data-ttu-id="13047-224">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="13047-224">residenceAddress</span></span>     | [<span data-ttu-id="13047-225">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="13047-225">physicalAddress</span></span>](../resources/physicaladdress.md)                 | <span data-ttu-id="13047-226">Endereço em que o usuário reside.</span><span class="sxs-lookup"><span data-stu-id="13047-226">Address where user lives.</span></span>                                                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="13047-227">student</span><span class="sxs-lookup"><span data-stu-id="13047-227">student</span></span>              | [<span data-ttu-id="13047-228">educationStudent</span><span class="sxs-lookup"><span data-stu-id="13047-228">educationStudent</span></span>](../resources/educationstudent.md)               | <span data-ttu-id="13047-229">Se a função principal for aluno, esse bloco conterá dados específicos do aluno.</span><span class="sxs-lookup"><span data-stu-id="13047-229">If the primary role is student, this block will contain student specific data.</span></span>                                                                                                                                                                                                                                                                              |
| <span data-ttu-id="13047-230">surname</span><span class="sxs-lookup"><span data-stu-id="13047-230">surname</span></span>              | <span data-ttu-id="13047-231">String</span><span class="sxs-lookup"><span data-stu-id="13047-231">String</span></span>                                                             | <span data-ttu-id="13047-p119">O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="13047-p119">The user's surname (family name or last name). Supports $filter.</span></span>                                                                                                                                                                                                                                                                                            |
| <span data-ttu-id="13047-234">teacher</span><span class="sxs-lookup"><span data-stu-id="13047-234">teacher</span></span>              | [<span data-ttu-id="13047-235">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="13047-235">educationTeacher</span></span>](../resources/educationteacher.md)               | <span data-ttu-id="13047-236">Se a função primária for professor, esse bloco conterá dados específicos do professor.</span><span class="sxs-lookup"><span data-stu-id="13047-236">If the primary role is teacher, this block will contain teacher specific data.</span></span>                                                                                                                                                                                                                                                                              |
| <span data-ttu-id="13047-237">usageLocation</span><span class="sxs-lookup"><span data-stu-id="13047-237">usageLocation</span></span>        | <span data-ttu-id="13047-238">String</span><span class="sxs-lookup"><span data-stu-id="13047-238">String</span></span>                                                             | <span data-ttu-id="13047-239">Um código de país de duas letras (padrão ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="13047-239">A two-letter country code (ISO standard 3166).</span></span> <span data-ttu-id="13047-240">Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços em países ou regiões.</span><span class="sxs-lookup"><span data-stu-id="13047-240">Required for users who will be assigned licenses due to a legal requirement to check for availability of services in countries or regions.</span></span> <span data-ttu-id="13047-241">Os exemplos incluem: "US", "JP" e "GB".</span><span class="sxs-lookup"><span data-stu-id="13047-241">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="13047-242">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="13047-242">Not nullable.</span></span> <span data-ttu-id="13047-243">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="13047-243">Supports $filter.</span></span>                                                                                           |
| <span data-ttu-id="13047-244">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="13047-244">userPrincipalName</span></span>    | <span data-ttu-id="13047-245">String</span><span class="sxs-lookup"><span data-stu-id="13047-245">String</span></span>                                                             | <span data-ttu-id="13047-246">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="13047-246">The user principal name (UPN) of the user.</span></span>                                                                                                                                                                                                                                                                                                                  |
| <span data-ttu-id="13047-247">userType</span><span class="sxs-lookup"><span data-stu-id="13047-247">userType</span></span>             | <span data-ttu-id="13047-248">String</span><span class="sxs-lookup"><span data-stu-id="13047-248">String</span></span>                                                             | <span data-ttu-id="13047-p121">Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como "Member" e "Guest". Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="13047-p121">A string value that can be used to classify user types in your directory, such as "Member" and "Guest". Supports $filter.</span></span>                                                                                                                                                                                                                                   |

## <a name="response"></a><span data-ttu-id="13047-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="13047-251">Response</span></span>

<span data-ttu-id="13047-252">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13047-252">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13047-253">Exemplos</span><span class="sxs-lookup"><span data-stu-id="13047-253">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13047-254">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13047-254">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/users
Content-Type: application/json
Content-length: 1585

{
  "@odata.type": "#microsoft.graph.educationUser",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```

### <a name="response"></a><span data-ttu-id="13047-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="13047-255">Response</span></span>

> <span data-ttu-id="13047-256">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="13047-256">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```
