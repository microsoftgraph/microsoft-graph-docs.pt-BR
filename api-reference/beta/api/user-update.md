---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1662290791eb996d74f045a032d5f1b581121205
ms.sourcegitcommit: 8ef30790a4d7aa94879df93773eae80b37abbfa4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37203967"
---
# <a name="update-user"></a><span data-ttu-id="0f4d3-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="0f4d3-103">Update user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f4d3-104">Atualizar as propriedades de um objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="0f4d3-104">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f4d3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f4d3-105">Permissions</span></span>
<span data-ttu-id="0f4d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f4d3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f4d3-108">Permission type</span></span>      | <span data-ttu-id="0f4d3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f4d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f4d3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f4d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f4d3-111">User. ReadWrite, User. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0f4d3-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f4d3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f4d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f4d3-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f4d3-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="0f4d3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f4d3-114">Application</span></span> | <span data-ttu-id="0f4d3-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f4d3-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="0f4d3-116">Ao atualizar a propriedade **passwordProfile** , a seguinte permissão é necessária: Directory. AccessAsUser. All.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-116">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="0f4d3-117">A atualização da propriedade **businessPhones**, **mobilePhone**ou **otherMails** de outro usuário só é permitida em usuários que não são administradores ou que recebem uma das seguintes funções: leitores de diretório, convidados convidados, leitor de centro de mensagens e Leitor de relatórios.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="0f4d3-118">Para obter mais detalhes, consulte administrador técnico (senha) no [Azure ad available Roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="0f4d3-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="0f4d3-119">Esse é o caso para aplicativos que receberam o User. ReadWrite. All ou Directory. ReadWrite. All delegad ou permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="0f4d3-120">A atualização da propriedade **Identities** requer a permissão User. ManageIdentities. All.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-120">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="0f4d3-121">Além disso, a adição de uma [conta local B2C](../resources/objectidentity.md) a um objeto de **usuário** existente não é permitida, a menos que o objeto **User** já contenha uma identidade de conta local.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-121">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="0f4d3-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4d3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="0f4d3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4d3-123">Request headers</span></span>
| <span data-ttu-id="0f4d3-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f4d3-124">Header</span></span>       | <span data-ttu-id="0f4d3-125">Valor</span><span class="sxs-lookup"><span data-stu-id="0f4d3-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="0f4d3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f4d3-126">Authorization</span></span>  | <span data-ttu-id="0f4d3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0f4d3-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f4d3-129">Content-Type</span></span>  | <span data-ttu-id="0f4d3-130">application/json</span><span class="sxs-lookup"><span data-stu-id="0f4d3-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f4d3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4d3-131">Request body</span></span>
<span data-ttu-id="0f4d3-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0f4d3-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f4d3-135">Property</span></span>     | <span data-ttu-id="0f4d3-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f4d3-136">Type</span></span>   |<span data-ttu-id="0f4d3-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f4d3-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f4d3-138">aboutMe</span><span class="sxs-lookup"><span data-stu-id="0f4d3-138">aboutMe</span></span>|<span data-ttu-id="0f4d3-139">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-139">String</span></span>|<span data-ttu-id="0f4d3-140">Um campo de entrada de texto em forma livre para o usuário se descrever.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-140">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="0f4d3-141">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="0f4d3-141">accountEnabled</span></span>|<span data-ttu-id="0f4d3-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f4d3-142">Boolean</span></span>| <span data-ttu-id="0f4d3-143">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-143">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="0f4d3-144">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-144">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="0f4d3-145">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="0f4d3-145">assignedLicenses</span></span>|<span data-ttu-id="0f4d3-146">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0f4d3-146">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="0f4d3-p107">As licenças que são atribuídas ao usuário. Não anulável.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p107">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="0f4d3-149">birthday</span><span class="sxs-lookup"><span data-stu-id="0f4d3-149">birthday</span></span>|<span data-ttu-id="0f4d3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f4d3-150">DateTimeOffset</span></span>|<span data-ttu-id="0f4d3-p108">O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p108">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0f4d3-154">businessPhones</span><span class="sxs-lookup"><span data-stu-id="0f4d3-154">businessPhones</span></span>| <span data-ttu-id="0f4d3-155">String collection</span><span class="sxs-lookup"><span data-stu-id="0f4d3-155">String collection</span></span> | <span data-ttu-id="0f4d3-p109">Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p109">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="0f4d3-158">city</span><span class="sxs-lookup"><span data-stu-id="0f4d3-158">city</span></span>|<span data-ttu-id="0f4d3-159">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-159">String</span></span>|<span data-ttu-id="0f4d3-160">A cidade em que o usuário está localizado.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-160">The city in which the user is located.</span></span>|
|<span data-ttu-id="0f4d3-161">country</span><span class="sxs-lookup"><span data-stu-id="0f4d3-161">country</span></span>|<span data-ttu-id="0f4d3-162">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-162">String</span></span>|<span data-ttu-id="0f4d3-163">O país/região no qual o usuário está localizado; por exemplo, "US" ou "ru".</span><span class="sxs-lookup"><span data-stu-id="0f4d3-163">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="0f4d3-164">department</span><span class="sxs-lookup"><span data-stu-id="0f4d3-164">department</span></span>|<span data-ttu-id="0f4d3-165">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-165">String</span></span>|<span data-ttu-id="0f4d3-166">O nome do departamento no qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-166">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="0f4d3-167">displayName</span><span class="sxs-lookup"><span data-stu-id="0f4d3-167">displayName</span></span>|<span data-ttu-id="0f4d3-168">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-168">String</span></span>|<span data-ttu-id="0f4d3-p110">O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p110">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="0f4d3-173">employeeId</span><span class="sxs-lookup"><span data-stu-id="0f4d3-173">employeeId</span></span>|<span data-ttu-id="0f4d3-174">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-174">String</span></span>|<span data-ttu-id="0f4d3-175">O identificador de funcionário atribuído ao usuário pela organização.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-175">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="0f4d3-176">givenName</span><span class="sxs-lookup"><span data-stu-id="0f4d3-176">givenName</span></span>|<span data-ttu-id="0f4d3-177">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-177">String</span></span>|<span data-ttu-id="0f4d3-178">O nome fornecido (nome) do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-178">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="0f4d3-179">hireDate</span><span class="sxs-lookup"><span data-stu-id="0f4d3-179">hireDate</span></span>|<span data-ttu-id="0f4d3-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f4d3-180">DateTimeOffset</span></span>|<span data-ttu-id="0f4d3-p111">A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p111">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0f4d3-184">identidade</span><span class="sxs-lookup"><span data-stu-id="0f4d3-184">identities</span></span>|<span data-ttu-id="0f4d3-185">coleção [Objectidentity](../resources/objectidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0f4d3-185">[objectIdentity](../resources/objectidentity.md) collection</span></span>| <span data-ttu-id="0f4d3-186">Representa as identidades que podem ser usadas para entrar nesta conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-186">Represents the identities that can be used to sign in to this user account.</span></span> <span data-ttu-id="0f4d3-187">Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google e Microsoft, e vinculada a uma conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-187">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, and Microsoft, and tied to a user account.</span></span> <span data-ttu-id="0f4d3-188">Qualquer atualização de **identidades** substituirá a coleção inteira e você deverá fornecer a identidade **signInType** userPrincipalName na coleção.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-188">Any update to **identities** will replace the entire collection and you must supply the userPrincipalName **signInType** identity in the collection.</span></span>|
|<span data-ttu-id="0f4d3-189">interests</span><span class="sxs-lookup"><span data-stu-id="0f4d3-189">interests</span></span>|<span data-ttu-id="0f4d3-190">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f4d3-190">String collection</span></span>|<span data-ttu-id="0f4d3-191">Uma lista para o usuário descrever os interesses dele.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-191">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="0f4d3-192">jobTitle</span><span class="sxs-lookup"><span data-stu-id="0f4d3-192">jobTitle</span></span>|<span data-ttu-id="0f4d3-193">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-193">String</span></span>|<span data-ttu-id="0f4d3-194">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-194">The user’s job title.</span></span>|
|<span data-ttu-id="0f4d3-195">mailNickname</span><span class="sxs-lookup"><span data-stu-id="0f4d3-195">mailNickname</span></span>|<span data-ttu-id="0f4d3-196">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-196">String</span></span>|<span data-ttu-id="0f4d3-197">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-197">The mail alias for the user.</span></span> <span data-ttu-id="0f4d3-198">Essa propriedade deve ser especificada quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-198">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="0f4d3-199">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="0f4d3-199">mobilePhone</span></span>|<span data-ttu-id="0f4d3-200">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-200">String</span></span>|<span data-ttu-id="0f4d3-201">O número de celular principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-201">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="0f4d3-202">mySite</span><span class="sxs-lookup"><span data-stu-id="0f4d3-202">mySite</span></span>|<span data-ttu-id="0f4d3-203">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-203">String</span></span>|<span data-ttu-id="0f4d3-204">A URL do site pessoal do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-204">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="0f4d3-205">officeLocation</span><span class="sxs-lookup"><span data-stu-id="0f4d3-205">officeLocation</span></span>|<span data-ttu-id="0f4d3-206">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-206">String</span></span>|<span data-ttu-id="0f4d3-207">A localização do escritório no local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-207">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="0f4d3-208">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="0f4d3-208">onPremisesImmutableId</span></span>|<span data-ttu-id="0f4d3-209">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-209">String</span></span>|<span data-ttu-id="0f4d3-210">Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-210">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="0f4d3-211">Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-211">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="0f4d3-212">**Importante:** Os caracteres **$** e **_** não podem ser usados ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-212">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="0f4d3-213">otherMails</span><span class="sxs-lookup"><span data-stu-id="0f4d3-213">otherMails</span></span>|<span data-ttu-id="0f4d3-214">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-214">String</span></span> |<span data-ttu-id="0f4d3-215">Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-215">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="0f4d3-216">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="0f4d3-216">passwordPolicies</span></span>|<span data-ttu-id="0f4d3-217">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-217">String</span></span>|<span data-ttu-id="0f4d3-p115">Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p115">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="0f4d3-222">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="0f4d3-222">passwordProfile</span></span>|[<span data-ttu-id="0f4d3-223">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="0f4d3-223">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="0f4d3-p116">Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p116">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="0f4d3-229">pastProjects</span><span class="sxs-lookup"><span data-stu-id="0f4d3-229">pastProjects</span></span>|<span data-ttu-id="0f4d3-230">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f4d3-230">String collection</span></span>|<span data-ttu-id="0f4d3-231">Uma lista para o usuário enumerar seus projetos anteriores.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-231">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="0f4d3-232">postalCode</span><span class="sxs-lookup"><span data-stu-id="0f4d3-232">postalCode</span></span>|<span data-ttu-id="0f4d3-233">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-233">String</span></span>|<span data-ttu-id="0f4d3-p117">O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p117">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="0f4d3-237">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="0f4d3-237">preferredLanguage</span></span>|<span data-ttu-id="0f4d3-238">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-238">String</span></span>|<span data-ttu-id="0f4d3-p118">O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p118">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="0f4d3-241">responsibilities</span><span class="sxs-lookup"><span data-stu-id="0f4d3-241">responsibilities</span></span>|<span data-ttu-id="0f4d3-242">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f4d3-242">String collection</span></span>|<span data-ttu-id="0f4d3-243">Uma lista para o usuário enumerar suas responsabilidades.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-243">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="0f4d3-244">schools</span><span class="sxs-lookup"><span data-stu-id="0f4d3-244">schools</span></span>|<span data-ttu-id="0f4d3-245">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f4d3-245">String collection</span></span>|<span data-ttu-id="0f4d3-246">Uma lista para o usuário enumerar as escolas que ele frequentou.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-246">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="0f4d3-247">skills</span><span class="sxs-lookup"><span data-stu-id="0f4d3-247">skills</span></span>|<span data-ttu-id="0f4d3-248">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f4d3-248">String collection</span></span>|<span data-ttu-id="0f4d3-249">Uma lista para o usuário enumerar suas qualificações.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-249">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="0f4d3-250">state</span><span class="sxs-lookup"><span data-stu-id="0f4d3-250">state</span></span>|<span data-ttu-id="0f4d3-251">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-251">String</span></span>|<span data-ttu-id="0f4d3-252">O estado ou município no endereço do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-252">The state or province in the user's address.</span></span>|
|<span data-ttu-id="0f4d3-253">streetAddress</span><span class="sxs-lookup"><span data-stu-id="0f4d3-253">streetAddress</span></span>|<span data-ttu-id="0f4d3-254">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-254">String</span></span>|<span data-ttu-id="0f4d3-255">O endereço do local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-255">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="0f4d3-256">surname</span><span class="sxs-lookup"><span data-stu-id="0f4d3-256">surname</span></span>|<span data-ttu-id="0f4d3-257">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-257">String</span></span>|<span data-ttu-id="0f4d3-258">O sobrenome do usuário (nome de família ou sobrenome).</span><span class="sxs-lookup"><span data-stu-id="0f4d3-258">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="0f4d3-259">usageLocation</span><span class="sxs-lookup"><span data-stu-id="0f4d3-259">usageLocation</span></span>|<span data-ttu-id="0f4d3-260">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f4d3-260">String</span></span>|<span data-ttu-id="0f4d3-261">Um código de duas letras (padrão ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="0f4d3-261">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="0f4d3-262">Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-262">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="0f4d3-263">Entre os exemplos temos: "US", "JT" e "GB".</span><span class="sxs-lookup"><span data-stu-id="0f4d3-263">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="0f4d3-264">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-264">Not nullable.</span></span>|
|<span data-ttu-id="0f4d3-265">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0f4d3-265">userPrincipalName</span></span>|<span data-ttu-id="0f4d3-266">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f4d3-266">String</span></span>|<span data-ttu-id="0f4d3-p120">O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](../resources/organization.md). Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-p120">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="0f4d3-274">userType</span><span class="sxs-lookup"><span data-stu-id="0f4d3-274">userType</span></span>|<span data-ttu-id="0f4d3-275">String</span><span class="sxs-lookup"><span data-stu-id="0f4d3-275">String</span></span>|<span data-ttu-id="0f4d3-276">Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-276">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="0f4d3-277">Como o recurso de **usuário** oferece suporte a [extensões](/graph/extensibility-overview), você `PATCH` pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **usuário** existente.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-277">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="0f4d3-278">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f4d3-278">Response</span></span>

<span data-ttu-id="0f4d3-279">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-279">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0f4d3-280">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f4d3-280">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="0f4d3-281">Exemplo 1: atualizar propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="0f4d3-281">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="0f4d3-282">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4d3-282">Request</span></span>

<span data-ttu-id="0f4d3-283">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-283">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0f4d3-284">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4d3-284">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f4d3-285">C#</span><span class="sxs-lookup"><span data-stu-id="0f4d3-285">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f4d3-286">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f4d3-286">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f4d3-287">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0f4d3-287">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0f4d3-288">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f4d3-288">Response</span></span>

<span data-ttu-id="0f4d3-289">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-289">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="0f4d3-290">Exemplo 2: atualizar propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="0f4d3-290">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="0f4d3-291">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4d3-291">Request</span></span>

<span data-ttu-id="0f4d3-292">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-292">The following example shows a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0f4d3-293">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4d3-293">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f4d3-294">C#</span><span class="sxs-lookup"><span data-stu-id="0f4d3-294">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f4d3-295">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f4d3-295">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f4d3-296">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0f4d3-296">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0f4d3-297">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f4d3-297">Response</span></span>

<span data-ttu-id="0f4d3-298">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="0f4d3-298">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="0f4d3-299">Confira também</span><span class="sxs-lookup"><span data-stu-id="0f4d3-299">See also</span></span>

- [<span data-ttu-id="0f4d3-300">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="0f4d3-300">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0f4d3-301">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="0f4d3-301">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="0f4d3-302">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="0f4d3-302">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
