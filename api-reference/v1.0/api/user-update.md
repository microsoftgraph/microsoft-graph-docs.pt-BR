---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ffb7590aa3200559ac1c7ef5186e06edf5654b13
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292578"
---
# <a name="update-user"></a><span data-ttu-id="5ca1c-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="5ca1c-103">Update user</span></span>

<span data-ttu-id="5ca1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ca1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ca1c-105">Atualize as propriedades de um objeto user.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-105">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ca1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ca1c-106">Permissions</span></span>
<span data-ttu-id="5ca1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ca1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ca1c-109">Permission type</span></span>      | <span data-ttu-id="5ca1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ca1c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ca1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ca1c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ca1c-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ca1c-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ca1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ca1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ca1c-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ca1c-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="5ca1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ca1c-115">Application</span></span> | <span data-ttu-id="5ca1c-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca1c-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="5ca1c-117">Ao atualizar a propriedade **passwordProfile**, a seguinte permissão é necessária: Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="5ca1c-118">A atualização da propriedade **businessPhones**, **mobilePhone** ou **otherMails** de outro usuário é permitida apenas em usuários que não sejam administradores ou que tenham uma das seguintes funções: Leitor de Diretório, Emissor de Convites Independente, Leitor do Centro de Mensagens e Leitor de Relatórios.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="5ca1c-119">Para obter mais detalhes, confira Administrador de suporte técnico (senha) nas [funções disponíveis do Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="5ca1c-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="5ca1c-120">Esse é o caso de aplicativos que receberam as permissões User.ReadWrite.All ou Directory.ReadWrite.All delegadas ou de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="5ca1c-121">A atualização da propriedade **Identidades** exige a permissão User.ManageIdentities.All.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="5ca1c-122">Além disso, não é permitido adicionar uma [conta local B2C](../resources/objectidentity.md) a um objeto de **usuário** existente, a menos que o objeto de **usuário** já tenha uma identidade de conta local.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="5ca1c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca1c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="5ca1c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca1c-124">Request headers</span></span>
| <span data-ttu-id="5ca1c-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ca1c-125">Header</span></span>       | <span data-ttu-id="5ca1c-126">Valor</span><span class="sxs-lookup"><span data-stu-id="5ca1c-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="5ca1c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ca1c-127">Authorization</span></span>  | <span data-ttu-id="5ca1c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5ca1c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ca1c-130">Content-Type</span></span>  | <span data-ttu-id="5ca1c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5ca1c-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ca1c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca1c-132">Request body</span></span>
<span data-ttu-id="5ca1c-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5ca1c-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ca1c-136">Property</span></span>     | <span data-ttu-id="5ca1c-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ca1c-137">Type</span></span>   |<span data-ttu-id="5ca1c-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ca1c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ca1c-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="5ca1c-139">aboutMe</span></span>|<span data-ttu-id="5ca1c-140">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-140">String</span></span>|<span data-ttu-id="5ca1c-141">Um campo de entrada de texto em forma livre para o usuário se descrever.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="5ca1c-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="5ca1c-142">accountEnabled</span></span>|<span data-ttu-id="5ca1c-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ca1c-143">Boolean</span></span>| <span data-ttu-id="5ca1c-144">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="5ca1c-145">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="5ca1c-146">birthday</span><span class="sxs-lookup"><span data-stu-id="5ca1c-146">birthday</span></span>|<span data-ttu-id="5ca1c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ca1c-147">DateTimeOffset</span></span>|<span data-ttu-id="5ca1c-p107">O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5ca1c-151">businessPhones</span><span class="sxs-lookup"><span data-stu-id="5ca1c-151">businessPhones</span></span>| <span data-ttu-id="5ca1c-152">String collection</span><span class="sxs-lookup"><span data-stu-id="5ca1c-152">String collection</span></span> | <span data-ttu-id="5ca1c-p108">Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p108">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="5ca1c-155">city</span><span class="sxs-lookup"><span data-stu-id="5ca1c-155">city</span></span>|<span data-ttu-id="5ca1c-156">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-156">String</span></span>|<span data-ttu-id="5ca1c-157">A cidade em que o usuário está localizado.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-157">The city in which the user is located.</span></span>|
|<span data-ttu-id="5ca1c-158">country</span><span class="sxs-lookup"><span data-stu-id="5ca1c-158">country</span></span>|<span data-ttu-id="5ca1c-159">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-159">String</span></span>|<span data-ttu-id="5ca1c-160">País/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido".</span><span class="sxs-lookup"><span data-stu-id="5ca1c-160">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="5ca1c-161">department</span><span class="sxs-lookup"><span data-stu-id="5ca1c-161">department</span></span>|<span data-ttu-id="5ca1c-162">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-162">String</span></span>|<span data-ttu-id="5ca1c-163">O nome do departamento no qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-163">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="5ca1c-164">displayName</span><span class="sxs-lookup"><span data-stu-id="5ca1c-164">displayName</span></span>|<span data-ttu-id="5ca1c-165">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-165">String</span></span>|<span data-ttu-id="5ca1c-p109">O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p109">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="5ca1c-170">givenName</span><span class="sxs-lookup"><span data-stu-id="5ca1c-170">givenName</span></span>|<span data-ttu-id="5ca1c-171">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-171">String</span></span>|<span data-ttu-id="5ca1c-172">O nome fornecido (nome) do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-172">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="5ca1c-173">hireDate</span><span class="sxs-lookup"><span data-stu-id="5ca1c-173">hireDate</span></span>|<span data-ttu-id="5ca1c-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ca1c-174">DateTimeOffset</span></span>|<span data-ttu-id="5ca1c-p110">A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p110">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5ca1c-178">interests</span><span class="sxs-lookup"><span data-stu-id="5ca1c-178">interests</span></span>|<span data-ttu-id="5ca1c-179">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ca1c-179">String collection</span></span>|<span data-ttu-id="5ca1c-180">Uma lista para o usuário descrever os interesses dele.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-180">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="5ca1c-181">jobTitle</span><span class="sxs-lookup"><span data-stu-id="5ca1c-181">jobTitle</span></span>|<span data-ttu-id="5ca1c-182">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-182">String</span></span>|<span data-ttu-id="5ca1c-183">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-183">The user’s job title.</span></span>|
|<span data-ttu-id="5ca1c-184">email</span><span class="sxs-lookup"><span data-stu-id="5ca1c-184">mail</span></span>|<span data-ttu-id="5ca1c-185">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-185">String</span></span>|<span data-ttu-id="5ca1c-186">O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com".</span><span class="sxs-lookup"><span data-stu-id="5ca1c-186">The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com".</span></span> <span data-ttu-id="5ca1c-187">As alterações feitas nessa propriedade também atualizarão a coleção **proxyAddresses** do usuário para incluir o valor como um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-187">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span> <br><br><span data-ttu-id="5ca1c-188">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-188">Supports $filter.</span></span>|
|<span data-ttu-id="5ca1c-189">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5ca1c-189">mailNickname</span></span>|<span data-ttu-id="5ca1c-190">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-190">String</span></span>|<span data-ttu-id="5ca1c-191">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-191">The mail alias for the user.</span></span> <span data-ttu-id="5ca1c-192">Essa propriedade deve ser especificada quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-192">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="5ca1c-193">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="5ca1c-193">mobilePhone</span></span>|<span data-ttu-id="5ca1c-194">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-194">String</span></span>|<span data-ttu-id="5ca1c-195">O número de celular principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-195">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="5ca1c-196">mySite</span><span class="sxs-lookup"><span data-stu-id="5ca1c-196">mySite</span></span>|<span data-ttu-id="5ca1c-197">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-197">String</span></span>|<span data-ttu-id="5ca1c-198">A URL do site pessoal do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-198">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="5ca1c-199">officeLocation</span><span class="sxs-lookup"><span data-stu-id="5ca1c-199">officeLocation</span></span>|<span data-ttu-id="5ca1c-200">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-200">String</span></span>|<span data-ttu-id="5ca1c-201">A localização do escritório no local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-201">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="5ca1c-202">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="5ca1c-202">onPremisesImmutableId</span></span>|<span data-ttu-id="5ca1c-203">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-203">String</span></span>|<span data-ttu-id="5ca1c-204">Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-204">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="5ca1c-205">Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-205">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="5ca1c-206">**Importante:** Os caracteres **$** e **_** e não podem ser usados ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-206">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="5ca1c-207">otherMails</span><span class="sxs-lookup"><span data-stu-id="5ca1c-207">otherMails</span></span>|<span data-ttu-id="5ca1c-208">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-208">String</span></span> |<span data-ttu-id="5ca1c-209">Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-209">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="5ca1c-210">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="5ca1c-210">passwordPolicies</span></span>|<span data-ttu-id="5ca1c-211">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-211">String</span></span>|<span data-ttu-id="5ca1c-p114">Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p114">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="5ca1c-216">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="5ca1c-216">passwordProfile</span></span>|[<span data-ttu-id="5ca1c-217">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="5ca1c-217">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="5ca1c-218">Especifica o perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-218">Specifies the password profile for the user.</span></span> <span data-ttu-id="5ca1c-219">O perfil contém a senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-219">The profile contains the user’s password.</span></span> <span data-ttu-id="5ca1c-220">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-220">This property is required when a user is created.</span></span> <span data-ttu-id="5ca1c-221">A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-221">The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property.</span></span> <span data-ttu-id="5ca1c-222">Por padrão, é obrigatória uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-222">By default, a strong password is required.</span></span> <span data-ttu-id="5ca1c-223">Isto não pode ser usado para usuários federados.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-223">This cannot be used for federated users.</span></span>|
|<span data-ttu-id="5ca1c-224">pastProjects</span><span class="sxs-lookup"><span data-stu-id="5ca1c-224">pastProjects</span></span>|<span data-ttu-id="5ca1c-225">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ca1c-225">String collection</span></span>|<span data-ttu-id="5ca1c-226">Uma lista para o usuário enumerar seus projetos anteriores.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-226">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="5ca1c-227">postalCode</span><span class="sxs-lookup"><span data-stu-id="5ca1c-227">postalCode</span></span>|<span data-ttu-id="5ca1c-228">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-228">String</span></span>|<span data-ttu-id="5ca1c-p116">O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p116">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="5ca1c-232">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="5ca1c-232">preferredLanguage</span></span>|<span data-ttu-id="5ca1c-233">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-233">String</span></span>|<span data-ttu-id="5ca1c-p117">O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p117">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="5ca1c-236">responsibilities</span><span class="sxs-lookup"><span data-stu-id="5ca1c-236">responsibilities</span></span>|<span data-ttu-id="5ca1c-237">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ca1c-237">String collection</span></span>|<span data-ttu-id="5ca1c-238">Uma lista para o usuário enumerar suas responsabilidades.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-238">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="5ca1c-239">schools</span><span class="sxs-lookup"><span data-stu-id="5ca1c-239">schools</span></span>|<span data-ttu-id="5ca1c-240">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ca1c-240">String collection</span></span>|<span data-ttu-id="5ca1c-241">Uma lista para o usuário enumerar as escolas que ele frequentou.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-241">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="5ca1c-242">skills</span><span class="sxs-lookup"><span data-stu-id="5ca1c-242">skills</span></span>|<span data-ttu-id="5ca1c-243">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ca1c-243">String collection</span></span>|<span data-ttu-id="5ca1c-244">Uma lista para o usuário enumerar suas qualificações.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-244">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="5ca1c-245">state</span><span class="sxs-lookup"><span data-stu-id="5ca1c-245">state</span></span>|<span data-ttu-id="5ca1c-246">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-246">String</span></span>|<span data-ttu-id="5ca1c-247">O estado ou município no endereço do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-247">The state or province in the user's address.</span></span>|
|<span data-ttu-id="5ca1c-248">streetAddress</span><span class="sxs-lookup"><span data-stu-id="5ca1c-248">streetAddress</span></span>|<span data-ttu-id="5ca1c-249">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-249">String</span></span>|<span data-ttu-id="5ca1c-250">O endereço do local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-250">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="5ca1c-251">surname</span><span class="sxs-lookup"><span data-stu-id="5ca1c-251">surname</span></span>|<span data-ttu-id="5ca1c-252">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-252">String</span></span>|<span data-ttu-id="5ca1c-253">O sobrenome do usuário (nome de família ou sobrenome).</span><span class="sxs-lookup"><span data-stu-id="5ca1c-253">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="5ca1c-254">usageLocation</span><span class="sxs-lookup"><span data-stu-id="5ca1c-254">usageLocation</span></span>|<span data-ttu-id="5ca1c-255">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-255">String</span></span>|<span data-ttu-id="5ca1c-256">Um código de duas letras (padrão ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="5ca1c-256">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="5ca1c-257">Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-257">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="5ca1c-258">Os exemplos incluem: "US", "JP" e "GB".</span><span class="sxs-lookup"><span data-stu-id="5ca1c-258">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="5ca1c-259">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-259">Not nullable.</span></span>|
|<span data-ttu-id="5ca1c-260">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ca1c-260">userPrincipalName</span></span>|<span data-ttu-id="5ca1c-261">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-261">String</span></span>|<span data-ttu-id="5ca1c-p119">O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](../resources/organization.md). Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-p119">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="5ca1c-269">userType</span><span class="sxs-lookup"><span data-stu-id="5ca1c-269">userType</span></span>|<span data-ttu-id="5ca1c-270">String</span><span class="sxs-lookup"><span data-stu-id="5ca1c-270">String</span></span>|<span data-ttu-id="5ca1c-271">Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-271">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

> [!NOTE] 
> <span data-ttu-id="5ca1c-272">As propriedades a seguir não podem ser atualizadas usando um contexto somente de aplicativo: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** e **skills**.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-272">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="5ca1c-273">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca1c-273">Response</span></span>

<span data-ttu-id="5ca1c-274">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-274">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5ca1c-275">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ca1c-275">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="5ca1c-276">Exemplo 1: atualizar as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="5ca1c-276">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="5ca1c-277">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca1c-277">Request</span></span>

<span data-ttu-id="5ca1c-278">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-278">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ca1c-279">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca1c-279">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="5ca1c-280">C#</span><span class="sxs-lookup"><span data-stu-id="5ca1c-280">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ca1c-281">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ca1c-281">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ca1c-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ca1c-282">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ca1c-283">Java</span><span class="sxs-lookup"><span data-stu-id="5ca1c-283">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5ca1c-284">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca1c-284">Response</span></span>
<span data-ttu-id="5ca1c-285">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-285">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="5ca1c-286">Exemplo 2: atualizar as propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="5ca1c-286">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="5ca1c-287">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca1c-287">Request</span></span>

<span data-ttu-id="5ca1c-288">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-288">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ca1c-289">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca1c-289">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="5ca1c-290">C#</span><span class="sxs-lookup"><span data-stu-id="5ca1c-290">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ca1c-291">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ca1c-291">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ca1c-292">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ca1c-292">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ca1c-293">Java</span><span class="sxs-lookup"><span data-stu-id="5ca1c-293">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ca1c-294">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca1c-294">Response</span></span>

<span data-ttu-id="5ca1c-295">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca1c-295">The following example shows the response.</span></span>
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
