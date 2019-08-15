---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 79f6ec2c72271319548750a4637aff28dfbd7f02
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421775"
---
# <a name="update-user"></a><span data-ttu-id="80518-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="80518-103">Update user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80518-104">Atualizar as propriedades de um objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="80518-104">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80518-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="80518-105">Permissions</span></span>
<span data-ttu-id="80518-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80518-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80518-108">Permission type</span></span>      | <span data-ttu-id="80518-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80518-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80518-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80518-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80518-111">User. ReadWrite, User. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="80518-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="80518-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80518-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80518-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80518-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="80518-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80518-114">Application</span></span> | <span data-ttu-id="80518-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80518-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="80518-116">Ao atualizar a propriedade **passwordProfile** , a seguinte permissão é necessária: Directory. AccessAsUser. All.</span><span class="sxs-lookup"><span data-stu-id="80518-116">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="80518-117">A atualização da propriedade **businessPhones**, **mobilePhone**ou **otherMails** de outro usuário só é permitida em usuários que não são administradores ou que recebem uma das seguintes funções: leitores de diretório, convidados convidados, leitor de centro de mensagens e Leitor de relatórios.</span><span class="sxs-lookup"><span data-stu-id="80518-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="80518-118">Para obter mais detalhes, consulte administrador técnico (senha) no [Azure ad available Roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="80518-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="80518-119">Esse é o caso para aplicativos que receberam o User. ReadWrite. All ou Directory. ReadWrite. All delegad ou permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80518-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>


## <a name="http-request"></a><span data-ttu-id="80518-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80518-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="80518-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80518-121">Request headers</span></span>
| <span data-ttu-id="80518-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80518-122">Header</span></span>       | <span data-ttu-id="80518-123">Valor</span><span class="sxs-lookup"><span data-stu-id="80518-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="80518-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="80518-124">Authorization</span></span>  | <span data-ttu-id="80518-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80518-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="80518-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80518-127">Content-Type</span></span>  | <span data-ttu-id="80518-128">application/json</span><span class="sxs-lookup"><span data-stu-id="80518-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80518-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80518-129">Request body</span></span>
<span data-ttu-id="80518-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="80518-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="80518-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80518-133">Property</span></span>     | <span data-ttu-id="80518-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="80518-134">Type</span></span>   |<span data-ttu-id="80518-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="80518-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80518-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="80518-136">aboutMe</span></span>|<span data-ttu-id="80518-137">String</span><span class="sxs-lookup"><span data-stu-id="80518-137">String</span></span>|<span data-ttu-id="80518-138">Um campo de entrada de texto em forma livre para o usuário se descrever.</span><span class="sxs-lookup"><span data-stu-id="80518-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="80518-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="80518-139">accountEnabled</span></span>|<span data-ttu-id="80518-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="80518-140">Boolean</span></span>| <span data-ttu-id="80518-141">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="80518-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="80518-142">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="80518-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="80518-143">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="80518-143">assignedLicenses</span></span>|<span data-ttu-id="80518-144">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="80518-144">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="80518-p106">As licenças que são atribuídas ao usuário. Não anulável.</span><span class="sxs-lookup"><span data-stu-id="80518-p106">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="80518-147">birthday</span><span class="sxs-lookup"><span data-stu-id="80518-147">birthday</span></span>|<span data-ttu-id="80518-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80518-148">DateTimeOffset</span></span>|<span data-ttu-id="80518-p107">O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="80518-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="80518-152">businessPhones</span><span class="sxs-lookup"><span data-stu-id="80518-152">businessPhones</span></span>| <span data-ttu-id="80518-153">String collection</span><span class="sxs-lookup"><span data-stu-id="80518-153">String collection</span></span> | <span data-ttu-id="80518-p108">Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="80518-p108">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="80518-156">city</span><span class="sxs-lookup"><span data-stu-id="80518-156">city</span></span>|<span data-ttu-id="80518-157">String</span><span class="sxs-lookup"><span data-stu-id="80518-157">String</span></span>|<span data-ttu-id="80518-158">A cidade em que o usuário está localizado.</span><span class="sxs-lookup"><span data-stu-id="80518-158">The city in which the user is located.</span></span>|
|<span data-ttu-id="80518-159">country</span><span class="sxs-lookup"><span data-stu-id="80518-159">country</span></span>|<span data-ttu-id="80518-160">String</span><span class="sxs-lookup"><span data-stu-id="80518-160">String</span></span>|<span data-ttu-id="80518-161">O país/região no qual o usuário está localizado; por exemplo, "US" ou "ru".</span><span class="sxs-lookup"><span data-stu-id="80518-161">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="80518-162">department</span><span class="sxs-lookup"><span data-stu-id="80518-162">department</span></span>|<span data-ttu-id="80518-163">String</span><span class="sxs-lookup"><span data-stu-id="80518-163">String</span></span>|<span data-ttu-id="80518-164">O nome do departamento no qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="80518-164">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="80518-165">displayName</span><span class="sxs-lookup"><span data-stu-id="80518-165">displayName</span></span>|<span data-ttu-id="80518-166">String</span><span class="sxs-lookup"><span data-stu-id="80518-166">String</span></span>|<span data-ttu-id="80518-p109">O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="80518-p109">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="80518-171">employeeId</span><span class="sxs-lookup"><span data-stu-id="80518-171">employeeId</span></span>|<span data-ttu-id="80518-172">String</span><span class="sxs-lookup"><span data-stu-id="80518-172">String</span></span>|<span data-ttu-id="80518-173">O identificador de funcionário atribuído ao usuário pela organização.</span><span class="sxs-lookup"><span data-stu-id="80518-173">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="80518-174">givenName</span><span class="sxs-lookup"><span data-stu-id="80518-174">givenName</span></span>|<span data-ttu-id="80518-175">String</span><span class="sxs-lookup"><span data-stu-id="80518-175">String</span></span>|<span data-ttu-id="80518-176">O nome fornecido (nome) do usuário.</span><span class="sxs-lookup"><span data-stu-id="80518-176">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="80518-177">hireDate</span><span class="sxs-lookup"><span data-stu-id="80518-177">hireDate</span></span>|<span data-ttu-id="80518-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80518-178">DateTimeOffset</span></span>|<span data-ttu-id="80518-p110">A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="80518-p110">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="80518-182">interests</span><span class="sxs-lookup"><span data-stu-id="80518-182">interests</span></span>|<span data-ttu-id="80518-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="80518-183">String collection</span></span>|<span data-ttu-id="80518-184">Uma lista para o usuário descrever os interesses dele.</span><span class="sxs-lookup"><span data-stu-id="80518-184">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="80518-185">jobTitle</span><span class="sxs-lookup"><span data-stu-id="80518-185">jobTitle</span></span>|<span data-ttu-id="80518-186">String</span><span class="sxs-lookup"><span data-stu-id="80518-186">String</span></span>|<span data-ttu-id="80518-187">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="80518-187">The user’s job title.</span></span>|
|<span data-ttu-id="80518-188">mailNickname</span><span class="sxs-lookup"><span data-stu-id="80518-188">mailNickname</span></span>|<span data-ttu-id="80518-189">String</span><span class="sxs-lookup"><span data-stu-id="80518-189">String</span></span>|<span data-ttu-id="80518-190">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="80518-190">The mail alias for the user.</span></span> <span data-ttu-id="80518-191">Essa propriedade deve ser especificada quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="80518-191">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="80518-192">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="80518-192">mobilePhone</span></span>|<span data-ttu-id="80518-193">String</span><span class="sxs-lookup"><span data-stu-id="80518-193">String</span></span>|<span data-ttu-id="80518-194">O número de celular principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="80518-194">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="80518-195">mySite</span><span class="sxs-lookup"><span data-stu-id="80518-195">mySite</span></span>|<span data-ttu-id="80518-196">String</span><span class="sxs-lookup"><span data-stu-id="80518-196">String</span></span>|<span data-ttu-id="80518-197">A URL do site pessoal do usuário.</span><span class="sxs-lookup"><span data-stu-id="80518-197">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="80518-198">officeLocation</span><span class="sxs-lookup"><span data-stu-id="80518-198">officeLocation</span></span>|<span data-ttu-id="80518-199">String</span><span class="sxs-lookup"><span data-stu-id="80518-199">String</span></span>|<span data-ttu-id="80518-200">A localização do escritório no local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="80518-200">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="80518-201">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="80518-201">onPremisesImmutableId</span></span>|<span data-ttu-id="80518-202">String</span><span class="sxs-lookup"><span data-stu-id="80518-202">String</span></span>|<span data-ttu-id="80518-203">Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="80518-203">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="80518-204">Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="80518-204">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="80518-205">**Importante:** Os caracteres **$** e **_** não podem ser usados ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="80518-205">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="80518-206">otherMails</span><span class="sxs-lookup"><span data-stu-id="80518-206">otherMails</span></span>|<span data-ttu-id="80518-207">String</span><span class="sxs-lookup"><span data-stu-id="80518-207">String</span></span> |<span data-ttu-id="80518-208">Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="80518-208">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="80518-209">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="80518-209">passwordPolicies</span></span>|<span data-ttu-id="80518-210">String</span><span class="sxs-lookup"><span data-stu-id="80518-210">String</span></span>|<span data-ttu-id="80518-p113">Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="80518-p113">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="80518-215">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="80518-215">passwordProfile</span></span>|[<span data-ttu-id="80518-216">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="80518-216">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="80518-p114">Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="80518-p114">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="80518-222">pastProjects</span><span class="sxs-lookup"><span data-stu-id="80518-222">pastProjects</span></span>|<span data-ttu-id="80518-223">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="80518-223">String collection</span></span>|<span data-ttu-id="80518-224">Uma lista para o usuário enumerar seus projetos anteriores.</span><span class="sxs-lookup"><span data-stu-id="80518-224">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="80518-225">postalCode</span><span class="sxs-lookup"><span data-stu-id="80518-225">postalCode</span></span>|<span data-ttu-id="80518-226">String</span><span class="sxs-lookup"><span data-stu-id="80518-226">String</span></span>|<span data-ttu-id="80518-p115">O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.</span><span class="sxs-lookup"><span data-stu-id="80518-p115">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="80518-230">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="80518-230">preferredLanguage</span></span>|<span data-ttu-id="80518-231">String</span><span class="sxs-lookup"><span data-stu-id="80518-231">String</span></span>|<span data-ttu-id="80518-p116">O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".</span><span class="sxs-lookup"><span data-stu-id="80518-p116">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="80518-234">responsibilities</span><span class="sxs-lookup"><span data-stu-id="80518-234">responsibilities</span></span>|<span data-ttu-id="80518-235">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="80518-235">String collection</span></span>|<span data-ttu-id="80518-236">Uma lista para o usuário enumerar suas responsabilidades.</span><span class="sxs-lookup"><span data-stu-id="80518-236">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="80518-237">schools</span><span class="sxs-lookup"><span data-stu-id="80518-237">schools</span></span>|<span data-ttu-id="80518-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="80518-238">String collection</span></span>|<span data-ttu-id="80518-239">Uma lista para o usuário enumerar as escolas que ele frequentou.</span><span class="sxs-lookup"><span data-stu-id="80518-239">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="80518-240">skills</span><span class="sxs-lookup"><span data-stu-id="80518-240">skills</span></span>|<span data-ttu-id="80518-241">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="80518-241">String collection</span></span>|<span data-ttu-id="80518-242">Uma lista para o usuário enumerar suas qualificações.</span><span class="sxs-lookup"><span data-stu-id="80518-242">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="80518-243">state</span><span class="sxs-lookup"><span data-stu-id="80518-243">state</span></span>|<span data-ttu-id="80518-244">String</span><span class="sxs-lookup"><span data-stu-id="80518-244">String</span></span>|<span data-ttu-id="80518-245">O estado ou município no endereço do usuário.</span><span class="sxs-lookup"><span data-stu-id="80518-245">The state or province in the user's address.</span></span>|
|<span data-ttu-id="80518-246">streetAddress</span><span class="sxs-lookup"><span data-stu-id="80518-246">streetAddress</span></span>|<span data-ttu-id="80518-247">String</span><span class="sxs-lookup"><span data-stu-id="80518-247">String</span></span>|<span data-ttu-id="80518-248">O endereço do local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="80518-248">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="80518-249">surname</span><span class="sxs-lookup"><span data-stu-id="80518-249">surname</span></span>|<span data-ttu-id="80518-250">String</span><span class="sxs-lookup"><span data-stu-id="80518-250">String</span></span>|<span data-ttu-id="80518-251">O sobrenome do usuário (nome de família ou sobrenome).</span><span class="sxs-lookup"><span data-stu-id="80518-251">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="80518-252">usageLocation</span><span class="sxs-lookup"><span data-stu-id="80518-252">usageLocation</span></span>|<span data-ttu-id="80518-253">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80518-253">String</span></span>|<span data-ttu-id="80518-254">Um código de duas letras (padrão ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="80518-254">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="80518-255">Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.</span><span class="sxs-lookup"><span data-stu-id="80518-255">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="80518-256">Entre os exemplos temos: "US", "JT" e "GB".</span><span class="sxs-lookup"><span data-stu-id="80518-256">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="80518-257">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="80518-257">Not nullable.</span></span>|
|<span data-ttu-id="80518-258">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="80518-258">userPrincipalName</span></span>|<span data-ttu-id="80518-259">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80518-259">String</span></span>|<span data-ttu-id="80518-p118">O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](../resources/organization.md). Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="80518-p118">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="80518-267">userType</span><span class="sxs-lookup"><span data-stu-id="80518-267">userType</span></span>|<span data-ttu-id="80518-268">String</span><span class="sxs-lookup"><span data-stu-id="80518-268">String</span></span>|<span data-ttu-id="80518-269">Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”.</span><span class="sxs-lookup"><span data-stu-id="80518-269">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="80518-270">Como o recurso de **usuário** oferece suporte a [extensões](/graph/extensibility-overview), você `PATCH` pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **usuário** existente.</span><span class="sxs-lookup"><span data-stu-id="80518-270">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="80518-271">Resposta</span><span class="sxs-lookup"><span data-stu-id="80518-271">Response</span></span>

<span data-ttu-id="80518-272">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80518-272">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80518-273">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80518-273">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="80518-274">Exemplo 1: atualizar propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="80518-274">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="80518-275">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80518-275">Request</span></span>

<span data-ttu-id="80518-276">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="80518-276">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="80518-277">HTTP</span><span class="sxs-lookup"><span data-stu-id="80518-277">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="80518-278">C#</span><span class="sxs-lookup"><span data-stu-id="80518-278">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80518-279">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80518-279">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80518-280">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="80518-280">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="80518-281">Resposta</span><span class="sxs-lookup"><span data-stu-id="80518-281">Response</span></span>

<span data-ttu-id="80518-282">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="80518-282">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="80518-283">Exemplo 2: atualizar propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="80518-283">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="80518-284">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80518-284">Request</span></span>

<span data-ttu-id="80518-285">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="80518-285">The following example shows a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="80518-286">HTTP</span><span class="sxs-lookup"><span data-stu-id="80518-286">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="80518-287">C#</span><span class="sxs-lookup"><span data-stu-id="80518-287">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80518-288">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80518-288">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80518-289">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="80518-289">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="80518-290">Resposta</span><span class="sxs-lookup"><span data-stu-id="80518-290">Response</span></span>

<span data-ttu-id="80518-291">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="80518-291">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="80518-292">Confira também</span><span class="sxs-lookup"><span data-stu-id="80518-292">See also</span></span>

- [<span data-ttu-id="80518-293">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="80518-293">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="80518-294">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="80518-294">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="80518-295">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="80518-295">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
