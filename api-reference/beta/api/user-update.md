---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4ba017109a761afb1606c55039601739781568de
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459564"
---
# <a name="update-user"></a><span data-ttu-id="beb25-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="beb25-103">Update user</span></span>

<span data-ttu-id="beb25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beb25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beb25-105">Atualizar as propriedades de um objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="beb25-105">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="beb25-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="beb25-106">Permissions</span></span>
<span data-ttu-id="beb25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beb25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beb25-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="beb25-109">Permission type</span></span>      | <span data-ttu-id="beb25-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="beb25-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beb25-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="beb25-111">Delegated (work or school account)</span></span> | <span data-ttu-id="beb25-112">User. ReadWrite, User. ReadWrite. All, User. ManageIdentities. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="beb25-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="beb25-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="beb25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beb25-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="beb25-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="beb25-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb25-115">Application</span></span> | <span data-ttu-id="beb25-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb25-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="beb25-117">Ao atualizar a propriedade **passwordProfile**, a seguinte permissão é necessária: Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="beb25-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="beb25-118">A atualização da propriedade **businessPhones**, **mobilePhone** ou **otherMails** de outro usuário é permitida apenas em usuários que não sejam administradores ou que tenham uma das seguintes funções: Leitor de Diretório, Emissor de Convites Independente, Leitor do Centro de Mensagens e Leitor de Relatórios.</span><span class="sxs-lookup"><span data-stu-id="beb25-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="beb25-119">Para obter mais detalhes, confira Administrador de suporte técnico (senha) nas [funções disponíveis do Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="beb25-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="beb25-120">Esse é o caso de aplicativos que receberam as permissões User.ReadWrite.All ou Directory.ReadWrite.All delegadas ou de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="beb25-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="beb25-121">A atualização da propriedade **Identidades** exige a permissão User.ManageIdentities.All.</span><span class="sxs-lookup"><span data-stu-id="beb25-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="beb25-122">Além disso, não é permitido adicionar uma [conta local B2C](../resources/objectidentity.md) a um objeto de **usuário** existente, a menos que o objeto de **usuário** já tenha uma identidade de conta local.</span><span class="sxs-lookup"><span data-stu-id="beb25-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="beb25-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="beb25-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="beb25-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="beb25-124">Request headers</span></span>
| <span data-ttu-id="beb25-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="beb25-125">Header</span></span>       | <span data-ttu-id="beb25-126">Valor</span><span class="sxs-lookup"><span data-stu-id="beb25-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="beb25-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="beb25-127">Authorization</span></span>  | <span data-ttu-id="beb25-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="beb25-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="beb25-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="beb25-130">Content-Type</span></span>  | <span data-ttu-id="beb25-131">application/json</span><span class="sxs-lookup"><span data-stu-id="beb25-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="beb25-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="beb25-132">Request body</span></span>
<span data-ttu-id="beb25-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="beb25-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="beb25-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="beb25-136">Property</span></span>     | <span data-ttu-id="beb25-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="beb25-137">Type</span></span>   |<span data-ttu-id="beb25-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="beb25-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="beb25-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="beb25-139">aboutMe</span></span>|<span data-ttu-id="beb25-140">String</span><span class="sxs-lookup"><span data-stu-id="beb25-140">String</span></span>|<span data-ttu-id="beb25-141">Um campo de entrada de texto em forma livre para o usuário se descrever.</span><span class="sxs-lookup"><span data-stu-id="beb25-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="beb25-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="beb25-142">accountEnabled</span></span>|<span data-ttu-id="beb25-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="beb25-143">Boolean</span></span>| <span data-ttu-id="beb25-144">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="beb25-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="beb25-145">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="beb25-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="beb25-146">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="beb25-146">assignedLicenses</span></span>|<span data-ttu-id="beb25-147">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="beb25-147">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="beb25-p107">As licenças que são atribuídas ao usuário. Não anulável.</span><span class="sxs-lookup"><span data-stu-id="beb25-p107">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="beb25-150">birthday</span><span class="sxs-lookup"><span data-stu-id="beb25-150">birthday</span></span>|<span data-ttu-id="beb25-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beb25-151">DateTimeOffset</span></span>|<span data-ttu-id="beb25-p108">O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="beb25-p108">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="beb25-155">businessPhones</span><span class="sxs-lookup"><span data-stu-id="beb25-155">businessPhones</span></span>| <span data-ttu-id="beb25-156">String collection</span><span class="sxs-lookup"><span data-stu-id="beb25-156">String collection</span></span> | <span data-ttu-id="beb25-p109">Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="beb25-p109">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="beb25-159">city</span><span class="sxs-lookup"><span data-stu-id="beb25-159">city</span></span>|<span data-ttu-id="beb25-160">String</span><span class="sxs-lookup"><span data-stu-id="beb25-160">String</span></span>|<span data-ttu-id="beb25-161">A cidade em que o usuário está localizado.</span><span class="sxs-lookup"><span data-stu-id="beb25-161">The city in which the user is located.</span></span>|
|<span data-ttu-id="beb25-162">country</span><span class="sxs-lookup"><span data-stu-id="beb25-162">country</span></span>|<span data-ttu-id="beb25-163">String</span><span class="sxs-lookup"><span data-stu-id="beb25-163">String</span></span>|<span data-ttu-id="beb25-164">País/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido".</span><span class="sxs-lookup"><span data-stu-id="beb25-164">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="beb25-165">department</span><span class="sxs-lookup"><span data-stu-id="beb25-165">department</span></span>|<span data-ttu-id="beb25-166">String</span><span class="sxs-lookup"><span data-stu-id="beb25-166">String</span></span>|<span data-ttu-id="beb25-167">O nome do departamento no qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="beb25-167">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="beb25-168">displayName</span><span class="sxs-lookup"><span data-stu-id="beb25-168">displayName</span></span>|<span data-ttu-id="beb25-169">String</span><span class="sxs-lookup"><span data-stu-id="beb25-169">String</span></span>|<span data-ttu-id="beb25-p110">O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="beb25-p110">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="beb25-174">employeeId</span><span class="sxs-lookup"><span data-stu-id="beb25-174">employeeId</span></span>|<span data-ttu-id="beb25-175">String</span><span class="sxs-lookup"><span data-stu-id="beb25-175">String</span></span>|<span data-ttu-id="beb25-176">O identificador de funcionário atribuído ao usuário pela organização.</span><span class="sxs-lookup"><span data-stu-id="beb25-176">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="beb25-177">givenName</span><span class="sxs-lookup"><span data-stu-id="beb25-177">givenName</span></span>|<span data-ttu-id="beb25-178">String</span><span class="sxs-lookup"><span data-stu-id="beb25-178">String</span></span>|<span data-ttu-id="beb25-179">O nome fornecido (nome) do usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-179">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="beb25-180">hireDate</span><span class="sxs-lookup"><span data-stu-id="beb25-180">hireDate</span></span>|<span data-ttu-id="beb25-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beb25-181">DateTimeOffset</span></span>|<span data-ttu-id="beb25-p111">A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="beb25-p111">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="beb25-185">Identidades</span><span class="sxs-lookup"><span data-stu-id="beb25-185">identities</span></span>|<span data-ttu-id="beb25-186">Coleção [objectIdentity](../resources/objectidentity.md)</span><span class="sxs-lookup"><span data-stu-id="beb25-186">[objectIdentity](../resources/objectidentity.md) collection</span></span>| <span data-ttu-id="beb25-187">Representa as identidades que podem ser usadas para entrar nesta conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-187">Represents the identities that can be used to sign in to this user account.</span></span> <span data-ttu-id="beb25-188">Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como o Facebook, Google e Microsoft, e está vinculada a uma conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-188">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, and Microsoft, and tied to a user account.</span></span> <span data-ttu-id="beb25-189">Qualquer atualização de **identidades** substituirá a coleção inteira e você deverá fornecer a identidade **signInType** userPrincipalName na coleção.</span><span class="sxs-lookup"><span data-stu-id="beb25-189">Any update to **identities** will replace the entire collection and you must supply the userPrincipalName **signInType** identity in the collection.</span></span>|
|<span data-ttu-id="beb25-190">interests</span><span class="sxs-lookup"><span data-stu-id="beb25-190">interests</span></span>|<span data-ttu-id="beb25-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="beb25-191">String collection</span></span>|<span data-ttu-id="beb25-192">Uma lista para o usuário descrever os interesses dele.</span><span class="sxs-lookup"><span data-stu-id="beb25-192">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="beb25-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="beb25-193">jobTitle</span></span>|<span data-ttu-id="beb25-194">String</span><span class="sxs-lookup"><span data-stu-id="beb25-194">String</span></span>|<span data-ttu-id="beb25-195">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-195">The user’s job title.</span></span>|
|<span data-ttu-id="beb25-196">email</span><span class="sxs-lookup"><span data-stu-id="beb25-196">mail</span></span>|<span data-ttu-id="beb25-197">String</span><span class="sxs-lookup"><span data-stu-id="beb25-197">String</span></span>|<span data-ttu-id="beb25-198">O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com".</span><span class="sxs-lookup"><span data-stu-id="beb25-198">The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com".</span></span> <span data-ttu-id="beb25-199">As alterações feitas nessa propriedade também atualizarão a coleção **proxyAddresses** do usuário para incluir o valor como um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="beb25-199">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span> <br><br><span data-ttu-id="beb25-200">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="beb25-200">Returned by default.</span></span> <span data-ttu-id="beb25-201">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="beb25-201">Supports $filter.</span></span>|
|<span data-ttu-id="beb25-202">mailNickname</span><span class="sxs-lookup"><span data-stu-id="beb25-202">mailNickname</span></span>|<span data-ttu-id="beb25-203">String</span><span class="sxs-lookup"><span data-stu-id="beb25-203">String</span></span>|<span data-ttu-id="beb25-204">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-204">The mail alias for the user.</span></span> <span data-ttu-id="beb25-205">Essa propriedade deve ser especificada quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="beb25-205">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="beb25-206">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="beb25-206">mobilePhone</span></span>|<span data-ttu-id="beb25-207">String</span><span class="sxs-lookup"><span data-stu-id="beb25-207">String</span></span>|<span data-ttu-id="beb25-208">O número de celular principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-208">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="beb25-209">mySite</span><span class="sxs-lookup"><span data-stu-id="beb25-209">mySite</span></span>|<span data-ttu-id="beb25-210">String</span><span class="sxs-lookup"><span data-stu-id="beb25-210">String</span></span>|<span data-ttu-id="beb25-211">A URL do site pessoal do usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-211">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="beb25-212">officeLocation</span><span class="sxs-lookup"><span data-stu-id="beb25-212">officeLocation</span></span>|<span data-ttu-id="beb25-213">String</span><span class="sxs-lookup"><span data-stu-id="beb25-213">String</span></span>|<span data-ttu-id="beb25-214">A localização do escritório no local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-214">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="beb25-215">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="beb25-215">onPremisesImmutableId</span></span>|<span data-ttu-id="beb25-216">String</span><span class="sxs-lookup"><span data-stu-id="beb25-216">String</span></span>|<span data-ttu-id="beb25-217">Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="beb25-217">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="beb25-218">Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-218">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="beb25-219">**Importante:** Os caracteres **$** e **_** e não podem ser usados ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="beb25-219">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="beb25-220">otherMails</span><span class="sxs-lookup"><span data-stu-id="beb25-220">otherMails</span></span>|<span data-ttu-id="beb25-221">String</span><span class="sxs-lookup"><span data-stu-id="beb25-221">String</span></span> |<span data-ttu-id="beb25-222">Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="beb25-222">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="beb25-223">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="beb25-223">passwordPolicies</span></span>|<span data-ttu-id="beb25-224">String</span><span class="sxs-lookup"><span data-stu-id="beb25-224">String</span></span>|<span data-ttu-id="beb25-p117">Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="beb25-p117">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="beb25-229">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="beb25-229">passwordProfile</span></span>|[<span data-ttu-id="beb25-230">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="beb25-230">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="beb25-p118">Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="beb25-p118">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="beb25-236">pastProjects</span><span class="sxs-lookup"><span data-stu-id="beb25-236">pastProjects</span></span>|<span data-ttu-id="beb25-237">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="beb25-237">String collection</span></span>|<span data-ttu-id="beb25-238">Uma lista para o usuário enumerar seus projetos anteriores.</span><span class="sxs-lookup"><span data-stu-id="beb25-238">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="beb25-239">postalCode</span><span class="sxs-lookup"><span data-stu-id="beb25-239">postalCode</span></span>|<span data-ttu-id="beb25-240">String</span><span class="sxs-lookup"><span data-stu-id="beb25-240">String</span></span>|<span data-ttu-id="beb25-p119">O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.</span><span class="sxs-lookup"><span data-stu-id="beb25-p119">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="beb25-244">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="beb25-244">preferredLanguage</span></span>|<span data-ttu-id="beb25-245">String</span><span class="sxs-lookup"><span data-stu-id="beb25-245">String</span></span>|<span data-ttu-id="beb25-p120">O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".</span><span class="sxs-lookup"><span data-stu-id="beb25-p120">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="beb25-248">responsibilities</span><span class="sxs-lookup"><span data-stu-id="beb25-248">responsibilities</span></span>|<span data-ttu-id="beb25-249">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="beb25-249">String collection</span></span>|<span data-ttu-id="beb25-250">Uma lista para o usuário enumerar suas responsabilidades.</span><span class="sxs-lookup"><span data-stu-id="beb25-250">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="beb25-251">schools</span><span class="sxs-lookup"><span data-stu-id="beb25-251">schools</span></span>|<span data-ttu-id="beb25-252">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="beb25-252">String collection</span></span>|<span data-ttu-id="beb25-253">Uma lista para o usuário enumerar as escolas que ele frequentou.</span><span class="sxs-lookup"><span data-stu-id="beb25-253">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="beb25-254">skills</span><span class="sxs-lookup"><span data-stu-id="beb25-254">skills</span></span>|<span data-ttu-id="beb25-255">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="beb25-255">String collection</span></span>|<span data-ttu-id="beb25-256">Uma lista para o usuário enumerar suas qualificações.</span><span class="sxs-lookup"><span data-stu-id="beb25-256">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="beb25-257">state</span><span class="sxs-lookup"><span data-stu-id="beb25-257">state</span></span>|<span data-ttu-id="beb25-258">String</span><span class="sxs-lookup"><span data-stu-id="beb25-258">String</span></span>|<span data-ttu-id="beb25-259">O estado ou município no endereço do usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-259">The state or province in the user's address.</span></span>|
|<span data-ttu-id="beb25-260">streetAddress</span><span class="sxs-lookup"><span data-stu-id="beb25-260">streetAddress</span></span>|<span data-ttu-id="beb25-261">String</span><span class="sxs-lookup"><span data-stu-id="beb25-261">String</span></span>|<span data-ttu-id="beb25-262">O endereço do local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="beb25-262">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="beb25-263">surname</span><span class="sxs-lookup"><span data-stu-id="beb25-263">surname</span></span>|<span data-ttu-id="beb25-264">String</span><span class="sxs-lookup"><span data-stu-id="beb25-264">String</span></span>|<span data-ttu-id="beb25-265">O sobrenome do usuário (nome de família ou sobrenome).</span><span class="sxs-lookup"><span data-stu-id="beb25-265">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="beb25-266">usageLocation</span><span class="sxs-lookup"><span data-stu-id="beb25-266">usageLocation</span></span>|<span data-ttu-id="beb25-267">String</span><span class="sxs-lookup"><span data-stu-id="beb25-267">String</span></span>|<span data-ttu-id="beb25-268">Um código de duas letras (padrão ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="beb25-268">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="beb25-269">Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.</span><span class="sxs-lookup"><span data-stu-id="beb25-269">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="beb25-270">Os exemplos incluem: "US", "JP" e "GB".</span><span class="sxs-lookup"><span data-stu-id="beb25-270">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="beb25-271">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="beb25-271">Not nullable.</span></span>|
|<span data-ttu-id="beb25-272">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="beb25-272">userPrincipalName</span></span>|<span data-ttu-id="beb25-273">String</span><span class="sxs-lookup"><span data-stu-id="beb25-273">String</span></span>|<span data-ttu-id="beb25-p122">O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](../resources/organization.md). Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="beb25-p122">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="beb25-281">userType</span><span class="sxs-lookup"><span data-stu-id="beb25-281">userType</span></span>|<span data-ttu-id="beb25-282">String</span><span class="sxs-lookup"><span data-stu-id="beb25-282">String</span></span>|<span data-ttu-id="beb25-283">Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”.</span><span class="sxs-lookup"><span data-stu-id="beb25-283">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="beb25-284">Como o recurso de **usuário** oferece suporte a [extensões](/graph/extensibility-overview), você pode usar a `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **usuário** existente.</span><span class="sxs-lookup"><span data-stu-id="beb25-284">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

> [!NOTE] 
> <span data-ttu-id="beb25-285">As propriedades a seguir não podem ser atualizadas usando um contexto somente de aplicativo: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** e **skills**.</span><span class="sxs-lookup"><span data-stu-id="beb25-285">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="beb25-286">Resposta</span><span class="sxs-lookup"><span data-stu-id="beb25-286">Response</span></span>

<span data-ttu-id="beb25-287">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="beb25-287">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="beb25-288">Exemplo</span><span class="sxs-lookup"><span data-stu-id="beb25-288">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="beb25-289">Exemplo 1: atualizar as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="beb25-289">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="beb25-290">Solicitação</span><span class="sxs-lookup"><span data-stu-id="beb25-290">Request</span></span>

<span data-ttu-id="beb25-291">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="beb25-291">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="beb25-292">HTTP</span><span class="sxs-lookup"><span data-stu-id="beb25-292">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="beb25-293">C#</span><span class="sxs-lookup"><span data-stu-id="beb25-293">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="beb25-294">JavaScript</span><span class="sxs-lookup"><span data-stu-id="beb25-294">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="beb25-295">Objective-C</span><span class="sxs-lookup"><span data-stu-id="beb25-295">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="beb25-296">Resposta</span><span class="sxs-lookup"><span data-stu-id="beb25-296">Response</span></span>

<span data-ttu-id="beb25-297">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="beb25-297">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="beb25-298">Exemplo 2: atualizar as propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="beb25-298">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="beb25-299">Solicitação</span><span class="sxs-lookup"><span data-stu-id="beb25-299">Request</span></span>

<span data-ttu-id="beb25-300">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="beb25-300">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="beb25-301">HTTP</span><span class="sxs-lookup"><span data-stu-id="beb25-301">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="beb25-302">C#</span><span class="sxs-lookup"><span data-stu-id="beb25-302">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="beb25-303">JavaScript</span><span class="sxs-lookup"><span data-stu-id="beb25-303">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="beb25-304">Objective-C</span><span class="sxs-lookup"><span data-stu-id="beb25-304">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="beb25-305">Resposta</span><span class="sxs-lookup"><span data-stu-id="beb25-305">Response</span></span>

<span data-ttu-id="beb25-306">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="beb25-306">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="beb25-307">Confira também</span><span class="sxs-lookup"><span data-stu-id="beb25-307">See also</span></span>

- [<span data-ttu-id="beb25-308">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="beb25-308">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="beb25-309">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="beb25-309">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="beb25-310">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="beb25-310">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
