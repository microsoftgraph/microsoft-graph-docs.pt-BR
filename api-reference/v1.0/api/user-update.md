---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0aef89c30fc67132352d9d70f9b0fc56e3a9063e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508902"
---
# <a name="update-user"></a><span data-ttu-id="b8668-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="b8668-103">Update user</span></span>

<span data-ttu-id="b8668-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8668-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8668-105">Atualize as propriedades de um objeto user.</span><span class="sxs-lookup"><span data-stu-id="b8668-105">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8668-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8668-106">Permissions</span></span>
<span data-ttu-id="b8668-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8668-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8668-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8668-109">Permission type</span></span>      | <span data-ttu-id="b8668-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8668-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8668-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8668-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b8668-112">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8668-112">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b8668-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8668-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8668-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8668-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="b8668-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8668-115">Application</span></span> | <span data-ttu-id="b8668-116">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8668-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="b8668-117">Ao atualizar a propriedade **passwordProfile**, a seguinte permissão é necessária: Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="b8668-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="b8668-118">A atualização da propriedade **businessPhones**, **mobilePhone** ou **otherMails** de outro usuário é permitida apenas em usuários que não sejam administradores ou que tenham uma das seguintes funções: Leitor de Diretório, Emissor de Convites Independente, Leitor do Centro de Mensagens e Leitor de Relatórios.</span><span class="sxs-lookup"><span data-stu-id="b8668-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="b8668-119">Para obter mais detalhes, confira Administrador de suporte técnico (senha) nas [funções disponíveis do Azure AD](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="b8668-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="b8668-120">Esse é o caso de aplicativos que receberam as permissões User.ReadWrite.All ou Directory.ReadWrite.All delegadas ou de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b8668-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="b8668-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8668-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="b8668-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8668-122">Request headers</span></span>
| <span data-ttu-id="b8668-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8668-123">Header</span></span>       | <span data-ttu-id="b8668-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b8668-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b8668-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8668-125">Authorization</span></span>  | <span data-ttu-id="b8668-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8668-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b8668-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8668-128">Content-Type</span></span>  | <span data-ttu-id="b8668-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b8668-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8668-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8668-130">Request body</span></span>
<span data-ttu-id="b8668-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b8668-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b8668-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8668-134">Property</span></span>     | <span data-ttu-id="b8668-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8668-135">Type</span></span>   |<span data-ttu-id="b8668-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8668-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8668-137">aboutMe</span><span class="sxs-lookup"><span data-stu-id="b8668-137">aboutMe</span></span>|<span data-ttu-id="b8668-138">String</span><span class="sxs-lookup"><span data-stu-id="b8668-138">String</span></span>|<span data-ttu-id="b8668-139">Um campo de entrada de texto em forma livre para o usuário se descrever.</span><span class="sxs-lookup"><span data-stu-id="b8668-139">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="b8668-140">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="b8668-140">accountEnabled</span></span>|<span data-ttu-id="b8668-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8668-141">Boolean</span></span>| <span data-ttu-id="b8668-142">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="b8668-142">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="b8668-143">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="b8668-143">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="b8668-144">birthday</span><span class="sxs-lookup"><span data-stu-id="b8668-144">birthday</span></span>|<span data-ttu-id="b8668-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8668-145">DateTimeOffset</span></span>|<span data-ttu-id="b8668-p106">O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b8668-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b8668-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="b8668-149">businessPhones</span></span>| <span data-ttu-id="b8668-150">String collection</span><span class="sxs-lookup"><span data-stu-id="b8668-150">String collection</span></span> | <span data-ttu-id="b8668-p107">Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="b8668-p107">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="b8668-153">city</span><span class="sxs-lookup"><span data-stu-id="b8668-153">city</span></span>|<span data-ttu-id="b8668-154">String</span><span class="sxs-lookup"><span data-stu-id="b8668-154">String</span></span>|<span data-ttu-id="b8668-155">A cidade em que o usuário está localizado.</span><span class="sxs-lookup"><span data-stu-id="b8668-155">The city in which the user is located.</span></span>|
|<span data-ttu-id="b8668-156">country</span><span class="sxs-lookup"><span data-stu-id="b8668-156">country</span></span>|<span data-ttu-id="b8668-157">String</span><span class="sxs-lookup"><span data-stu-id="b8668-157">String</span></span>|<span data-ttu-id="b8668-158">País/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido".</span><span class="sxs-lookup"><span data-stu-id="b8668-158">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="b8668-159">department</span><span class="sxs-lookup"><span data-stu-id="b8668-159">department</span></span>|<span data-ttu-id="b8668-160">String</span><span class="sxs-lookup"><span data-stu-id="b8668-160">String</span></span>|<span data-ttu-id="b8668-161">O nome do departamento no qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="b8668-161">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="b8668-162">displayName</span><span class="sxs-lookup"><span data-stu-id="b8668-162">displayName</span></span>|<span data-ttu-id="b8668-163">String</span><span class="sxs-lookup"><span data-stu-id="b8668-163">String</span></span>|<span data-ttu-id="b8668-p108">O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="b8668-p108">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="b8668-168">givenName</span><span class="sxs-lookup"><span data-stu-id="b8668-168">givenName</span></span>|<span data-ttu-id="b8668-169">String</span><span class="sxs-lookup"><span data-stu-id="b8668-169">String</span></span>|<span data-ttu-id="b8668-170">O nome fornecido (nome) do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8668-170">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="b8668-171">hireDate</span><span class="sxs-lookup"><span data-stu-id="b8668-171">hireDate</span></span>|<span data-ttu-id="b8668-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8668-172">DateTimeOffset</span></span>|<span data-ttu-id="b8668-p109">A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b8668-p109">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b8668-176">interests</span><span class="sxs-lookup"><span data-stu-id="b8668-176">interests</span></span>|<span data-ttu-id="b8668-177">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8668-177">String collection</span></span>|<span data-ttu-id="b8668-178">Uma lista para o usuário descrever os interesses dele.</span><span class="sxs-lookup"><span data-stu-id="b8668-178">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="b8668-179">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b8668-179">jobTitle</span></span>|<span data-ttu-id="b8668-180">String</span><span class="sxs-lookup"><span data-stu-id="b8668-180">String</span></span>|<span data-ttu-id="b8668-181">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8668-181">The user’s job title.</span></span>|
|<span data-ttu-id="b8668-182">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b8668-182">mailNickname</span></span>|<span data-ttu-id="b8668-183">String</span><span class="sxs-lookup"><span data-stu-id="b8668-183">String</span></span>|<span data-ttu-id="b8668-184">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8668-184">The mail alias for the user.</span></span> <span data-ttu-id="b8668-185">Essa propriedade deve ser especificada quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="b8668-185">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="b8668-186">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b8668-186">mobilePhone</span></span>|<span data-ttu-id="b8668-187">String</span><span class="sxs-lookup"><span data-stu-id="b8668-187">String</span></span>|<span data-ttu-id="b8668-188">O número de celular principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8668-188">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="b8668-189">mySite</span><span class="sxs-lookup"><span data-stu-id="b8668-189">mySite</span></span>|<span data-ttu-id="b8668-190">String</span><span class="sxs-lookup"><span data-stu-id="b8668-190">String</span></span>|<span data-ttu-id="b8668-191">A URL do site pessoal do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8668-191">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="b8668-192">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b8668-192">officeLocation</span></span>|<span data-ttu-id="b8668-193">String</span><span class="sxs-lookup"><span data-stu-id="b8668-193">String</span></span>|<span data-ttu-id="b8668-194">A localização do escritório no local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8668-194">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="b8668-195">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="b8668-195">onPremisesImmutableId</span></span>|<span data-ttu-id="b8668-196">String</span><span class="sxs-lookup"><span data-stu-id="b8668-196">String</span></span>|<span data-ttu-id="b8668-197">Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b8668-197">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="b8668-198">Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8668-198">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="b8668-199">**Importante:** Os caracteres **$** e **_** e não podem ser usados ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="b8668-199">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="b8668-200">otherMails</span><span class="sxs-lookup"><span data-stu-id="b8668-200">otherMails</span></span>|<span data-ttu-id="b8668-201">String</span><span class="sxs-lookup"><span data-stu-id="b8668-201">String</span></span> |<span data-ttu-id="b8668-202">Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="b8668-202">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="b8668-203">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="b8668-203">passwordPolicies</span></span>|<span data-ttu-id="b8668-204">String</span><span class="sxs-lookup"><span data-stu-id="b8668-204">String</span></span>|<span data-ttu-id="b8668-p112">Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="b8668-p112">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="b8668-209">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="b8668-209">passwordProfile</span></span>|[<span data-ttu-id="b8668-210">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="b8668-210">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="b8668-p113">Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="b8668-p113">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="b8668-216">pastProjects</span><span class="sxs-lookup"><span data-stu-id="b8668-216">pastProjects</span></span>|<span data-ttu-id="b8668-217">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8668-217">String collection</span></span>|<span data-ttu-id="b8668-218">Uma lista para o usuário enumerar seus projetos anteriores.</span><span class="sxs-lookup"><span data-stu-id="b8668-218">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="b8668-219">postalCode</span><span class="sxs-lookup"><span data-stu-id="b8668-219">postalCode</span></span>|<span data-ttu-id="b8668-220">String</span><span class="sxs-lookup"><span data-stu-id="b8668-220">String</span></span>|<span data-ttu-id="b8668-p114">O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.</span><span class="sxs-lookup"><span data-stu-id="b8668-p114">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="b8668-224">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="b8668-224">preferredLanguage</span></span>|<span data-ttu-id="b8668-225">String</span><span class="sxs-lookup"><span data-stu-id="b8668-225">String</span></span>|<span data-ttu-id="b8668-p115">O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".</span><span class="sxs-lookup"><span data-stu-id="b8668-p115">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="b8668-228">responsibilities</span><span class="sxs-lookup"><span data-stu-id="b8668-228">responsibilities</span></span>|<span data-ttu-id="b8668-229">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8668-229">String collection</span></span>|<span data-ttu-id="b8668-230">Uma lista para o usuário enumerar suas responsabilidades.</span><span class="sxs-lookup"><span data-stu-id="b8668-230">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="b8668-231">schools</span><span class="sxs-lookup"><span data-stu-id="b8668-231">schools</span></span>|<span data-ttu-id="b8668-232">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8668-232">String collection</span></span>|<span data-ttu-id="b8668-233">Uma lista para o usuário enumerar as escolas que ele frequentou.</span><span class="sxs-lookup"><span data-stu-id="b8668-233">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="b8668-234">skills</span><span class="sxs-lookup"><span data-stu-id="b8668-234">skills</span></span>|<span data-ttu-id="b8668-235">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8668-235">String collection</span></span>|<span data-ttu-id="b8668-236">Uma lista para o usuário enumerar suas qualificações.</span><span class="sxs-lookup"><span data-stu-id="b8668-236">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="b8668-237">state</span><span class="sxs-lookup"><span data-stu-id="b8668-237">state</span></span>|<span data-ttu-id="b8668-238">String</span><span class="sxs-lookup"><span data-stu-id="b8668-238">String</span></span>|<span data-ttu-id="b8668-239">O estado ou município no endereço do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8668-239">The state or province in the user's address.</span></span>|
|<span data-ttu-id="b8668-240">streetAddress</span><span class="sxs-lookup"><span data-stu-id="b8668-240">streetAddress</span></span>|<span data-ttu-id="b8668-241">String</span><span class="sxs-lookup"><span data-stu-id="b8668-241">String</span></span>|<span data-ttu-id="b8668-242">O endereço do local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8668-242">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="b8668-243">surname</span><span class="sxs-lookup"><span data-stu-id="b8668-243">surname</span></span>|<span data-ttu-id="b8668-244">String</span><span class="sxs-lookup"><span data-stu-id="b8668-244">String</span></span>|<span data-ttu-id="b8668-245">O sobrenome do usuário (nome de família ou sobrenome).</span><span class="sxs-lookup"><span data-stu-id="b8668-245">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="b8668-246">usageLocation</span><span class="sxs-lookup"><span data-stu-id="b8668-246">usageLocation</span></span>|<span data-ttu-id="b8668-247">String</span><span class="sxs-lookup"><span data-stu-id="b8668-247">String</span></span>|<span data-ttu-id="b8668-248">Um código de duas letras (padrão ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="b8668-248">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="b8668-249">Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.</span><span class="sxs-lookup"><span data-stu-id="b8668-249">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="b8668-250">Os exemplos incluem: "US", "JP" e "GB".</span><span class="sxs-lookup"><span data-stu-id="b8668-250">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="b8668-251">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="b8668-251">Not nullable.</span></span>|
|<span data-ttu-id="b8668-252">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b8668-252">userPrincipalName</span></span>|<span data-ttu-id="b8668-253">String</span><span class="sxs-lookup"><span data-stu-id="b8668-253">String</span></span>|<span data-ttu-id="b8668-p117">O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](../resources/organization.md). Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="b8668-p117">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="b8668-261">userType</span><span class="sxs-lookup"><span data-stu-id="b8668-261">userType</span></span>|<span data-ttu-id="b8668-262">String</span><span class="sxs-lookup"><span data-stu-id="b8668-262">String</span></span>|<span data-ttu-id="b8668-263">Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”.</span><span class="sxs-lookup"><span data-stu-id="b8668-263">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="b8668-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8668-264">Response</span></span>

<span data-ttu-id="b8668-265">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8668-265">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8668-266">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8668-266">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="b8668-267">Exemplo 1: atualizar as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="b8668-267">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="b8668-268">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8668-268">Request</span></span>

<span data-ttu-id="b8668-269">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8668-269">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8668-270">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8668-270">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b8668-271">C#</span><span class="sxs-lookup"><span data-stu-id="b8668-271">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8668-272">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8668-272">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8668-273">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8668-273">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8668-274">Java</span><span class="sxs-lookup"><span data-stu-id="b8668-274">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b8668-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8668-275">Response</span></span>
<span data-ttu-id="b8668-276">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8668-276">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="b8668-277">Exemplo 2: atualizar as propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="b8668-277">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="b8668-278">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8668-278">Request</span></span>

<span data-ttu-id="b8668-279">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8668-279">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b8668-280">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8668-280">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b8668-281">C#</span><span class="sxs-lookup"><span data-stu-id="b8668-281">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8668-282">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8668-282">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8668-283">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8668-283">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8668-284">Java</span><span class="sxs-lookup"><span data-stu-id="b8668-284">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b8668-285">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8668-285">Response</span></span>

<span data-ttu-id="b8668-286">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8668-286">The following example shows the response.</span></span>
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
