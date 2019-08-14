---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: af8d2c99d814c8a7b82e905e3fbbc7d5709bb9d6
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396853"
---
# <a name="update-user"></a><span data-ttu-id="af270-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="af270-103">Update user</span></span>

<span data-ttu-id="af270-104">Atualize as propriedades de um objeto user.</span><span class="sxs-lookup"><span data-stu-id="af270-104">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="af270-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="af270-105">Permissions</span></span>
<span data-ttu-id="af270-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af270-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af270-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af270-108">Permission type</span></span>      | <span data-ttu-id="af270-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af270-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af270-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af270-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af270-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af270-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af270-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af270-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af270-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af270-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="af270-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af270-114">Application</span></span> | <span data-ttu-id="af270-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af270-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="af270-116">Ao atualizar a propriedade **passwordProfile**, a seguinte permissão é necessária: Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="af270-116">When updating the passwordProfile property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="af270-117">A atualização da propriedade **businessPhones**, **mobilePhone** ou **otherMails** de outro usuário é permitida apenas em usuários que não sejam administradores ou que tenham uma das seguintes funções: Leitor de Diretório, Emissor de Convites Independente, Leitor do Centro de Mensagens e Leitor de Relatórios.</span><span class="sxs-lookup"><span data-stu-id="af270-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="af270-118">Para obter mais detalhes, confira Administrador de suporte técnico (senha) nas [funções disponíveis do Azure AD](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="af270-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="af270-119">Esse é o caso de aplicativos que receberam as permissões User.ReadWrite.All ou Directory.ReadWrite.All delegadas ou de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="af270-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="af270-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af270-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="af270-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af270-121">Request headers</span></span>
| <span data-ttu-id="af270-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af270-122">Header</span></span>       | <span data-ttu-id="af270-123">Valor</span><span class="sxs-lookup"><span data-stu-id="af270-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="af270-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="af270-124">Authorization</span></span>  | <span data-ttu-id="af270-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af270-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af270-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af270-127">Content-Type</span></span>  | <span data-ttu-id="af270-128">application/json</span><span class="sxs-lookup"><span data-stu-id="af270-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af270-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af270-129">Request body</span></span>
<span data-ttu-id="af270-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="af270-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="af270-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af270-133">Property</span></span>     | <span data-ttu-id="af270-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="af270-134">Type</span></span>   |<span data-ttu-id="af270-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="af270-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af270-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="af270-136">aboutMe</span></span>|<span data-ttu-id="af270-137">String</span><span class="sxs-lookup"><span data-stu-id="af270-137">String</span></span>|<span data-ttu-id="af270-138">Um campo de entrada de texto em forma livre para o usuário se descrever.</span><span class="sxs-lookup"><span data-stu-id="af270-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="af270-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="af270-139">accountEnabled</span></span>|<span data-ttu-id="af270-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="af270-140">Boolean</span></span>| <span data-ttu-id="af270-141">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="af270-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="af270-142">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="af270-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="af270-143">birthday</span><span class="sxs-lookup"><span data-stu-id="af270-143">birthday</span></span>|<span data-ttu-id="af270-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af270-144">DateTimeOffset</span></span>|<span data-ttu-id="af270-p106">O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="af270-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="af270-148">businessPhones</span><span class="sxs-lookup"><span data-stu-id="af270-148">businessPhones</span></span>| <span data-ttu-id="af270-149">String collection</span><span class="sxs-lookup"><span data-stu-id="af270-149">String collection</span></span> | <span data-ttu-id="af270-p107">Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="af270-p107">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="af270-152">city</span><span class="sxs-lookup"><span data-stu-id="af270-152">city</span></span>|<span data-ttu-id="af270-153">String</span><span class="sxs-lookup"><span data-stu-id="af270-153">String</span></span>|<span data-ttu-id="af270-154">A cidade em que o usuário está localizado.</span><span class="sxs-lookup"><span data-stu-id="af270-154">The city in which the user is located.</span></span>|
|<span data-ttu-id="af270-155">country</span><span class="sxs-lookup"><span data-stu-id="af270-155">country</span></span>|<span data-ttu-id="af270-156">String</span><span class="sxs-lookup"><span data-stu-id="af270-156">String</span></span>|<span data-ttu-id="af270-157">País/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido".</span><span class="sxs-lookup"><span data-stu-id="af270-157">The country/region in which the user is located; for example, “US” or “UK”. Supports $filter.</span></span>|
|<span data-ttu-id="af270-158">department</span><span class="sxs-lookup"><span data-stu-id="af270-158">department</span></span>|<span data-ttu-id="af270-159">String</span><span class="sxs-lookup"><span data-stu-id="af270-159">String</span></span>|<span data-ttu-id="af270-160">O nome do departamento no qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="af270-160">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="af270-161">displayName</span><span class="sxs-lookup"><span data-stu-id="af270-161">displayName</span></span>|<span data-ttu-id="af270-162">String</span><span class="sxs-lookup"><span data-stu-id="af270-162">String</span></span>|<span data-ttu-id="af270-p108">O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="af270-p108">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="af270-167">givenName</span><span class="sxs-lookup"><span data-stu-id="af270-167">givenName</span></span>|<span data-ttu-id="af270-168">String</span><span class="sxs-lookup"><span data-stu-id="af270-168">String</span></span>|<span data-ttu-id="af270-169">O nome fornecido (nome) do usuário.</span><span class="sxs-lookup"><span data-stu-id="af270-169">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="af270-170">hireDate</span><span class="sxs-lookup"><span data-stu-id="af270-170">hireDate</span></span>|<span data-ttu-id="af270-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af270-171">DateTimeOffset</span></span>|<span data-ttu-id="af270-p109">A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="af270-p109">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="af270-175">interests</span><span class="sxs-lookup"><span data-stu-id="af270-175">interests</span></span>|<span data-ttu-id="af270-176">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="af270-176">String collection</span></span>|<span data-ttu-id="af270-177">Uma lista para o usuário descrever os interesses dele.</span><span class="sxs-lookup"><span data-stu-id="af270-177">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="af270-178">jobTitle</span><span class="sxs-lookup"><span data-stu-id="af270-178">jobTitle</span></span>|<span data-ttu-id="af270-179">String</span><span class="sxs-lookup"><span data-stu-id="af270-179">String</span></span>|<span data-ttu-id="af270-180">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="af270-180">The user’s job title.</span></span>|
|<span data-ttu-id="af270-181">mailNickname</span><span class="sxs-lookup"><span data-stu-id="af270-181">mailNickname</span></span>|<span data-ttu-id="af270-182">String</span><span class="sxs-lookup"><span data-stu-id="af270-182">String</span></span>|<span data-ttu-id="af270-183">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="af270-183">The mail alias for the user.</span></span> <span data-ttu-id="af270-184">Essa propriedade deve ser especificada quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="af270-184">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="af270-185">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="af270-185">mobilePhone</span></span>|<span data-ttu-id="af270-186">String</span><span class="sxs-lookup"><span data-stu-id="af270-186">String</span></span>|<span data-ttu-id="af270-187">O número de celular principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="af270-187">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="af270-188">mySite</span><span class="sxs-lookup"><span data-stu-id="af270-188">mySite</span></span>|<span data-ttu-id="af270-189">String</span><span class="sxs-lookup"><span data-stu-id="af270-189">String</span></span>|<span data-ttu-id="af270-190">A URL do site pessoal do usuário.</span><span class="sxs-lookup"><span data-stu-id="af270-190">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="af270-191">officeLocation</span><span class="sxs-lookup"><span data-stu-id="af270-191">officeLocation</span></span>|<span data-ttu-id="af270-192">String</span><span class="sxs-lookup"><span data-stu-id="af270-192">String</span></span>|<span data-ttu-id="af270-193">A localização do escritório no local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="af270-193">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="af270-194">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="af270-194">onPremisesImmutableId</span></span>|<span data-ttu-id="af270-195">String</span><span class="sxs-lookup"><span data-stu-id="af270-195">String</span></span>|<span data-ttu-id="af270-196">Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="af270-196">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="af270-197">Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="af270-197">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="af270-198">**Importante:** Os caracteres **$** e **_** e não podem ser usados ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="af270-198">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="af270-199">otherMails</span><span class="sxs-lookup"><span data-stu-id="af270-199">otherMails</span></span>|<span data-ttu-id="af270-200">String</span><span class="sxs-lookup"><span data-stu-id="af270-200">String</span></span> |<span data-ttu-id="af270-201">Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="af270-201">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="af270-202">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="af270-202">passwordPolicies</span></span>|<span data-ttu-id="af270-203">String</span><span class="sxs-lookup"><span data-stu-id="af270-203">String</span></span>|<span data-ttu-id="af270-p112">Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="af270-p112">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="af270-208">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="af270-208">passwordProfile</span></span>|[<span data-ttu-id="af270-209">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="af270-209">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="af270-p113">Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="af270-p113">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="af270-215">pastProjects</span><span class="sxs-lookup"><span data-stu-id="af270-215">pastProjects</span></span>|<span data-ttu-id="af270-216">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="af270-216">String collection</span></span>|<span data-ttu-id="af270-217">Uma lista para o usuário enumerar seus projetos anteriores.</span><span class="sxs-lookup"><span data-stu-id="af270-217">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="af270-218">postalCode</span><span class="sxs-lookup"><span data-stu-id="af270-218">postalCode</span></span>|<span data-ttu-id="af270-219">String</span><span class="sxs-lookup"><span data-stu-id="af270-219">String</span></span>|<span data-ttu-id="af270-p114">O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.</span><span class="sxs-lookup"><span data-stu-id="af270-p114">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="af270-223">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="af270-223">preferredLanguage</span></span>|<span data-ttu-id="af270-224">String</span><span class="sxs-lookup"><span data-stu-id="af270-224">String</span></span>|<span data-ttu-id="af270-p115">O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".</span><span class="sxs-lookup"><span data-stu-id="af270-p115">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="af270-227">responsibilities</span><span class="sxs-lookup"><span data-stu-id="af270-227">responsibilities</span></span>|<span data-ttu-id="af270-228">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="af270-228">String collection</span></span>|<span data-ttu-id="af270-229">Uma lista para o usuário enumerar suas responsabilidades.</span><span class="sxs-lookup"><span data-stu-id="af270-229">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="af270-230">schools</span><span class="sxs-lookup"><span data-stu-id="af270-230">schools</span></span>|<span data-ttu-id="af270-231">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="af270-231">String collection</span></span>|<span data-ttu-id="af270-232">Uma lista para o usuário enumerar as escolas que ele frequentou.</span><span class="sxs-lookup"><span data-stu-id="af270-232">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="af270-233">skills</span><span class="sxs-lookup"><span data-stu-id="af270-233">skills</span></span>|<span data-ttu-id="af270-234">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="af270-234">String collection</span></span>|<span data-ttu-id="af270-235">Uma lista para o usuário enumerar suas qualificações.</span><span class="sxs-lookup"><span data-stu-id="af270-235">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="af270-236">state</span><span class="sxs-lookup"><span data-stu-id="af270-236">state</span></span>|<span data-ttu-id="af270-237">String</span><span class="sxs-lookup"><span data-stu-id="af270-237">String</span></span>|<span data-ttu-id="af270-238">O estado ou município no endereço do usuário.</span><span class="sxs-lookup"><span data-stu-id="af270-238">The state or province in the user's address.</span></span>|
|<span data-ttu-id="af270-239">streetAddress</span><span class="sxs-lookup"><span data-stu-id="af270-239">streetAddress</span></span>|<span data-ttu-id="af270-240">String</span><span class="sxs-lookup"><span data-stu-id="af270-240">String</span></span>|<span data-ttu-id="af270-241">O endereço do local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="af270-241">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="af270-242">surname</span><span class="sxs-lookup"><span data-stu-id="af270-242">surname</span></span>|<span data-ttu-id="af270-243">String</span><span class="sxs-lookup"><span data-stu-id="af270-243">String</span></span>|<span data-ttu-id="af270-244">O sobrenome do usuário (nome de família ou sobrenome).</span><span class="sxs-lookup"><span data-stu-id="af270-244">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="af270-245">usageLocation</span><span class="sxs-lookup"><span data-stu-id="af270-245">usageLocation</span></span>|<span data-ttu-id="af270-246">String</span><span class="sxs-lookup"><span data-stu-id="af270-246">String</span></span>|<span data-ttu-id="af270-247">Um código de duas letras (padrão ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="af270-247">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="af270-248">Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.</span><span class="sxs-lookup"><span data-stu-id="af270-248">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="af270-249">Os exemplos incluem: "US", "JP" e "GB".</span><span class="sxs-lookup"><span data-stu-id="af270-249">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="af270-250">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="af270-250">Not nullable.</span></span>|
|<span data-ttu-id="af270-251">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af270-251">userPrincipalName</span></span>|<span data-ttu-id="af270-252">String</span><span class="sxs-lookup"><span data-stu-id="af270-252">String</span></span>|<span data-ttu-id="af270-p117">O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](../resources/organization.md). Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="af270-p117">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="af270-260">userType</span><span class="sxs-lookup"><span data-stu-id="af270-260">userType</span></span>|<span data-ttu-id="af270-261">String</span><span class="sxs-lookup"><span data-stu-id="af270-261">String</span></span>|<span data-ttu-id="af270-262">Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”.</span><span class="sxs-lookup"><span data-stu-id="af270-262">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="af270-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="af270-263">Response</span></span>

<span data-ttu-id="af270-264">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="af270-264">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="af270-265">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af270-265">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="af270-266">Exemplo 1: atualizar as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="af270-266">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="af270-267">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af270-267">Request</span></span>

<span data-ttu-id="af270-268">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="af270-268">The following example shows how to create a request context.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="af270-269">HTTP</span><span class="sxs-lookup"><span data-stu-id="af270-269">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="af270-270">C#</span><span class="sxs-lookup"><span data-stu-id="af270-270">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af270-271">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af270-271">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="af270-272">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af270-272">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="af270-273">Java</span><span class="sxs-lookup"><span data-stu-id="af270-273">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="af270-274">Resposta</span><span class="sxs-lookup"><span data-stu-id="af270-274">Response</span></span>
<span data-ttu-id="af270-275">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="af270-275">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="af270-276">Exemplo 2: atualizar as propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="af270-276">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="af270-277">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af270-277">Request</span></span>

<span data-ttu-id="af270-278">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="af270-278">The following example shows how to create a request context.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="af270-279">HTTP</span><span class="sxs-lookup"><span data-stu-id="af270-279">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="af270-280">C#</span><span class="sxs-lookup"><span data-stu-id="af270-280">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af270-281">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af270-281">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="af270-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af270-282">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="af270-283">Java</span><span class="sxs-lookup"><span data-stu-id="af270-283">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="af270-284">Resposta</span><span class="sxs-lookup"><span data-stu-id="af270-284">Response</span></span>

<span data-ttu-id="af270-285">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="af270-285">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
