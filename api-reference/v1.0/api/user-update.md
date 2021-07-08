---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 10578c33f55432122d9178c2e19f325b95b10fdb
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316509"
---
# <a name="update-user"></a><span data-ttu-id="e9504-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="e9504-103">Update user</span></span>

<span data-ttu-id="e9504-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9504-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9504-105">Atualizar as propriedades de um objeto [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="e9504-105">Update the properties of a [user](../resources/user.md) object.</span></span> <span data-ttu-id="e9504-106">Nem todas as propriedades podem ser atualizadas por usuários Membros ou Convidados com suas permissões padrão sem Funções de administrador.</span><span class="sxs-lookup"><span data-stu-id="e9504-106">Not all properties can be updated by Member or Guest users with their default permissions without Administrator roles.</span></span> <span data-ttu-id="e9504-107">[Compare as permissões padrão de membros e convidados](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) para ver as propriedades que eles podem gerenciar.</span><span class="sxs-lookup"><span data-stu-id="e9504-107">[Compare member and guest default permissions](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) to see properties they can manage.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9504-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9504-108">Permissions</span></span>
<span data-ttu-id="e9504-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9504-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9504-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9504-111">Permission type</span></span>      | <span data-ttu-id="e9504-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9504-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9504-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9504-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e9504-114">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9504-114">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e9504-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9504-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9504-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9504-116">User.ReadWrite</span></span>    |
|<span data-ttu-id="e9504-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9504-117">Application</span></span> | <span data-ttu-id="e9504-118">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9504-118">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="e9504-119">Ao atualizar a propriedade **passwordProfile**, a seguinte permissão é necessária: Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="e9504-119">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="e9504-120">A atualização da propriedade **businessPhones**, **mobilePhone** ou **otherMails** de outro usuário é permitida apenas em usuários que não sejam administradores ou que tenham uma das seguintes funções: Leitor de Diretório, Emissor de Convites Independente, Leitor do Centro de Mensagens e Leitor de Relatórios.</span><span class="sxs-lookup"><span data-stu-id="e9504-120">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="e9504-121">Para obter mais detalhes, confira Administrador de suporte técnico (senha) em [funções internas do Azure Active Directory](/azure/active-directory/roles/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9504-121">For more details, see Helpdesk (Password) Administrator in [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference).</span></span>  <span data-ttu-id="e9504-122">Esse é o caso de aplicativos que receberam as permissões User.ReadWrite.All ou Directory.ReadWrite.All delegadas ou de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e9504-122">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>
> - <span data-ttu-id="e9504-123">Sua conta Microsoft pessoal deve estar vinculada a um locatário do AAD para atualizar seu perfil com a permissão delegada User.ReadWrite em uma conta Microsoft pessoal.</span><span class="sxs-lookup"><span data-stu-id="e9504-123">Your personal Microsoft account must be tied to an AAD tenant to update your profile with the User.ReadWrite delegated permission on a personal Microsoft account.</span></span>
> - <span data-ttu-id="e9504-124">A atualização da propriedade **Identidades** exige a permissão User.ManageIdentities.All.</span><span class="sxs-lookup"><span data-stu-id="e9504-124">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="e9504-125">Além disso, não é permitido adicionar uma [conta local B2C](../resources/objectidentity.md) a um objeto de **usuário** existente, a menos que o objeto de **usuário** já tenha uma identidade de conta local.</span><span class="sxs-lookup"><span data-stu-id="e9504-125">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="e9504-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9504-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="e9504-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9504-127">Request headers</span></span>
| <span data-ttu-id="e9504-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9504-128">Header</span></span>       | <span data-ttu-id="e9504-129">Valor</span><span class="sxs-lookup"><span data-stu-id="e9504-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e9504-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9504-130">Authorization</span></span>  | <span data-ttu-id="e9504-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9504-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e9504-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9504-133">Content-Type</span></span>  | <span data-ttu-id="e9504-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e9504-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9504-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9504-135">Request body</span></span>
<span data-ttu-id="e9504-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e9504-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e9504-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9504-139">Property</span></span>     | <span data-ttu-id="e9504-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9504-140">Type</span></span>   |<span data-ttu-id="e9504-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9504-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9504-142">aboutMe</span><span class="sxs-lookup"><span data-stu-id="e9504-142">aboutMe</span></span>|<span data-ttu-id="e9504-143">String</span><span class="sxs-lookup"><span data-stu-id="e9504-143">String</span></span>|<span data-ttu-id="e9504-144">Um campo de entrada de texto em forma livre para o usuário se descrever.</span><span class="sxs-lookup"><span data-stu-id="e9504-144">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="e9504-145">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="e9504-145">accountEnabled</span></span>|<span data-ttu-id="e9504-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="e9504-146">Boolean</span></span>| <span data-ttu-id="e9504-147">`true` se a conta estiver habilitada; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="e9504-147">`true` if the account is enabled; otherwise, `false`.</span></span> <span data-ttu-id="e9504-148">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="e9504-148">This property is required when a user is created.</span></span>    |
| <span data-ttu-id="e9504-149">ageGroup</span><span class="sxs-lookup"><span data-stu-id="e9504-149">ageGroup</span></span> | [<span data-ttu-id="e9504-150">ageGroup</span><span class="sxs-lookup"><span data-stu-id="e9504-150">ageGroup</span></span>](../resources/user.md#agegroup-values) | <span data-ttu-id="e9504-151">Define a faixa etária do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-151">Sets the age group of the user.</span></span> <span data-ttu-id="e9504-152">Valores permitidos: `null`, `minor`, `notAdult` e `adult`.</span><span class="sxs-lookup"><span data-stu-id="e9504-152">Allowed values: `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="e9504-153">Confira as [definições de propriedades da faixa etária legal](../resources/user.md#legal-age-group-property-definitions) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e9504-153">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="e9504-154">birthday</span><span class="sxs-lookup"><span data-stu-id="e9504-154">birthday</span></span>|<span data-ttu-id="e9504-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9504-155">DateTimeOffset</span></span>|<span data-ttu-id="e9504-156">O aniversário do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-156">The birthday of the user.</span></span> <span data-ttu-id="e9504-157">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e9504-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9504-158">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="e9504-158">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e9504-159">businessPhones</span><span class="sxs-lookup"><span data-stu-id="e9504-159">businessPhones</span></span>| <span data-ttu-id="e9504-160">String collection</span><span class="sxs-lookup"><span data-stu-id="e9504-160">String collection</span></span> | <span data-ttu-id="e9504-p110">Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="e9504-p110">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="e9504-163">city</span><span class="sxs-lookup"><span data-stu-id="e9504-163">city</span></span>|<span data-ttu-id="e9504-164">String</span><span class="sxs-lookup"><span data-stu-id="e9504-164">String</span></span>|<span data-ttu-id="e9504-165">A cidade em que o usuário está localizado.</span><span class="sxs-lookup"><span data-stu-id="e9504-165">The city in which the user is located.</span></span>|
| <span data-ttu-id="e9504-166">companyName</span><span class="sxs-lookup"><span data-stu-id="e9504-166">companyName</span></span> | <span data-ttu-id="e9504-167">String</span><span class="sxs-lookup"><span data-stu-id="e9504-167">String</span></span> | <span data-ttu-id="e9504-168">O nome da empresa em que o usuário está associado.</span><span class="sxs-lookup"><span data-stu-id="e9504-168">The company name which the user is associated.</span></span> <span data-ttu-id="e9504-169">Essa propriedade pode ser útil para descrever a empresa de onde procede um usuário externo.</span><span class="sxs-lookup"><span data-stu-id="e9504-169">This property can be useful for describing the company that an external user comes from.</span></span> <span data-ttu-id="e9504-170">O comprimento máximo do nome da empresa é 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e9504-170">The maximum length of the company name is 64 characters.</span></span> |
| <span data-ttu-id="e9504-171">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="e9504-171">consentProvidedForMinor</span></span> | [<span data-ttu-id="e9504-172">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="e9504-172">consentProvidedForMinor</span></span>](../resources/user.md#consentprovidedforminor-values) | <span data-ttu-id="e9504-173">Define se o consentimento foi obtido para menores.</span><span class="sxs-lookup"><span data-stu-id="e9504-173">Sets whether consent has been obtained for minors.</span></span> <span data-ttu-id="e9504-174">Valores permitidos: `null`, `granted`, `denied` e `notRequired`.</span><span class="sxs-lookup"><span data-stu-id="e9504-174">Allowed values: `null`, `granted`, `denied` and `notRequired`.</span></span> <span data-ttu-id="e9504-175">Confira as [definições de propriedades da faixa etária legal](../resources/user.md#legal-age-group-property-definitions) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e9504-175">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="e9504-176">country</span><span class="sxs-lookup"><span data-stu-id="e9504-176">country</span></span>|<span data-ttu-id="e9504-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9504-177">String</span></span>|<span data-ttu-id="e9504-178">O país/região em que o usuário está localizado; por exemplo, `US` ou `UK`.</span><span class="sxs-lookup"><span data-stu-id="e9504-178">The country/region in which the user is located; for example, `US` or `UK`.</span></span>|
|<span data-ttu-id="e9504-179">department</span><span class="sxs-lookup"><span data-stu-id="e9504-179">department</span></span>|<span data-ttu-id="e9504-180">String</span><span class="sxs-lookup"><span data-stu-id="e9504-180">String</span></span>|<span data-ttu-id="e9504-181">O nome do departamento no qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="e9504-181">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="e9504-182">displayName</span><span class="sxs-lookup"><span data-stu-id="e9504-182">displayName</span></span>|<span data-ttu-id="e9504-183">String</span><span class="sxs-lookup"><span data-stu-id="e9504-183">String</span></span>|<span data-ttu-id="e9504-184">O nome exibido para o usuário no catálogo de endereços.</span><span class="sxs-lookup"><span data-stu-id="e9504-184">The name displayed in the address book for the user.</span></span> <span data-ttu-id="e9504-185">É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-185">This is usually the combination of the user's first name, middle initial and last name.</span></span> <span data-ttu-id="e9504-186">Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="e9504-186">This property is required when a user is created and it cannot be cleared during updates.</span></span> <span data-ttu-id="e9504-187">Oferece suporte para `$filter` e `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="e9504-187">Supports `$filter` and `$orderby`.</span></span>|
| <span data-ttu-id="e9504-188">employeeId</span><span class="sxs-lookup"><span data-stu-id="e9504-188">employeeId</span></span> | <span data-ttu-id="e9504-189">String</span><span class="sxs-lookup"><span data-stu-id="e9504-189">String</span></span> | <span data-ttu-id="e9504-190">O identificador de funcionário atribuído ao usuário pela organização.</span><span class="sxs-lookup"><span data-stu-id="e9504-190">The employee identifier assigned to the user by the organization.</span></span> |
| <span data-ttu-id="e9504-191">employeeType</span><span class="sxs-lookup"><span data-stu-id="e9504-191">employeeType</span></span> | <span data-ttu-id="e9504-192">String</span><span class="sxs-lookup"><span data-stu-id="e9504-192">String</span></span> | <span data-ttu-id="e9504-193">Captura o tipo de trabalhador corporativo.</span><span class="sxs-lookup"><span data-stu-id="e9504-193">Captures enterprise worker type.</span></span> <span data-ttu-id="e9504-194">Por exemplo, `Employee`, `Contractor`, `Consultant` ou `Vendor`.</span><span class="sxs-lookup"><span data-stu-id="e9504-194">For example, `Employee`, `Contractor`, `Consultant`, or `Vendor`.</span></span> <span data-ttu-id="e9504-195">Retornado apenas em `$select`.</span><span class="sxs-lookup"><span data-stu-id="e9504-195">Returned only on `$select`.</span></span>|
|<span data-ttu-id="e9504-196">givenName</span><span class="sxs-lookup"><span data-stu-id="e9504-196">givenName</span></span>|<span data-ttu-id="e9504-197">String</span><span class="sxs-lookup"><span data-stu-id="e9504-197">String</span></span>|<span data-ttu-id="e9504-198">O nome fornecido (nome) do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-198">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="e9504-199">hireDate</span><span class="sxs-lookup"><span data-stu-id="e9504-199">hireDate</span></span>|<span data-ttu-id="e9504-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9504-200">DateTimeOffset</span></span>|<span data-ttu-id="e9504-201">A data de contratação do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-201">The hire date of the user.</span></span> <span data-ttu-id="e9504-202">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e9504-202">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9504-203">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="e9504-203">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e9504-204">interests</span><span class="sxs-lookup"><span data-stu-id="e9504-204">interests</span></span>|<span data-ttu-id="e9504-205">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9504-205">String collection</span></span>|<span data-ttu-id="e9504-206">Uma lista para o usuário descrever os interesses dele.</span><span class="sxs-lookup"><span data-stu-id="e9504-206">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="e9504-207">jobTitle</span><span class="sxs-lookup"><span data-stu-id="e9504-207">jobTitle</span></span>|<span data-ttu-id="e9504-208">String</span><span class="sxs-lookup"><span data-stu-id="e9504-208">String</span></span>|<span data-ttu-id="e9504-209">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-209">The user’s job title.</span></span>|
|<span data-ttu-id="e9504-210">email</span><span class="sxs-lookup"><span data-stu-id="e9504-210">mail</span></span>|<span data-ttu-id="e9504-211">String</span><span class="sxs-lookup"><span data-stu-id="e9504-211">String</span></span>|<span data-ttu-id="e9504-212">O endereço SMTP do usuário, por exemplo, `jeff@contoso.onmicrosoft.com`.</span><span class="sxs-lookup"><span data-stu-id="e9504-212">The SMTP address for the user, for example, `jeff@contoso.onmicrosoft.com`.</span></span> <span data-ttu-id="e9504-213">As alterações feitas nessa propriedade também atualizarão a coleção **proxyAddresses** do usuário para incluir o valor como um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="e9504-213">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span>|
|<span data-ttu-id="e9504-214">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e9504-214">mailNickname</span></span>|<span data-ttu-id="e9504-215">String</span><span class="sxs-lookup"><span data-stu-id="e9504-215">String</span></span>|<span data-ttu-id="e9504-p117">O alias de e-mail do usuário. Essa propriedade deve ser especificada quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="e9504-p117">The mail alias for the user. This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="e9504-218">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="e9504-218">mobilePhone</span></span>|<span data-ttu-id="e9504-219">String</span><span class="sxs-lookup"><span data-stu-id="e9504-219">String</span></span>|<span data-ttu-id="e9504-220">O número de celular principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-220">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="e9504-221">mySite</span><span class="sxs-lookup"><span data-stu-id="e9504-221">mySite</span></span>|<span data-ttu-id="e9504-222">String</span><span class="sxs-lookup"><span data-stu-id="e9504-222">String</span></span>|<span data-ttu-id="e9504-223">A URL do site pessoal do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-223">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="e9504-224">officeLocation</span><span class="sxs-lookup"><span data-stu-id="e9504-224">officeLocation</span></span>|<span data-ttu-id="e9504-225">String</span><span class="sxs-lookup"><span data-stu-id="e9504-225">String</span></span>|<span data-ttu-id="e9504-226">A localização do escritório no local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-226">The office location in the user's place of business.</span></span>|
| <span data-ttu-id="e9504-227">onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="e9504-227">onPremisesExtensionAttributes</span></span> | [<span data-ttu-id="e9504-228">onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="e9504-228">onPremisesExtensionAttributes</span></span>](../resources/onpremisesextensionattributes.md) | <span data-ttu-id="e9504-229">Contém extensionAttributes 1-15 para o usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-229">Contains extensionAttributes 1-15 for the user.</span></span> <span data-ttu-id="e9504-230">Observe que os atributos de extensão individuais não são selecionáveis nem filtráveis.</span><span class="sxs-lookup"><span data-stu-id="e9504-230">Note that the individual extension attributes are neither selectable nor filterable.</span></span> <span data-ttu-id="e9504-231">Para um usuário do `onPremisesSyncEnabled`, a fonte de autoridade desse conjunto de propriedades é o local e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e9504-231">For an `onPremisesSyncEnabled` user, the source of authority for this set of properties is the on-premises and is read-only and is read-only.</span></span> <span data-ttu-id="e9504-232">Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="e9504-232">These extension attributes are also known as Exchange custom attributes 1-15.</span></span>|
|<span data-ttu-id="e9504-233">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="e9504-233">onPremisesImmutableId</span></span>|<span data-ttu-id="e9504-234">String</span><span class="sxs-lookup"><span data-stu-id="e9504-234">String</span></span>|<span data-ttu-id="e9504-235">Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9504-235">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="e9504-236">Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-236">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="e9504-237">**Importante:** Os caracteres **$** e **_** e não podem ser usados ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="e9504-237">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="e9504-238">otherMails</span><span class="sxs-lookup"><span data-stu-id="e9504-238">otherMails</span></span>|<span data-ttu-id="e9504-239">String</span><span class="sxs-lookup"><span data-stu-id="e9504-239">String</span></span> |<span data-ttu-id="e9504-240">Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="e9504-240">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="e9504-241">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="e9504-241">passwordPolicies</span></span>|<span data-ttu-id="e9504-242">String</span><span class="sxs-lookup"><span data-stu-id="e9504-242">String</span></span>|<span data-ttu-id="e9504-243">Especifica as políticas de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-243">Specifies password policies for the user.</span></span> <span data-ttu-id="e9504-244">Este valor é uma enumeração com um valor possível sendo `DisableStrongPassword`, que permite que senhas mais fracas do que a política padrão sejam especificadas.</span><span class="sxs-lookup"><span data-stu-id="e9504-244">This value is an enumeration with one possible value being `DisableStrongPassword`, which allows weaker passwords than the default policy to be specified.</span></span> <span data-ttu-id="e9504-245">`DisablePasswordExpiration` também pode ser especificado.</span><span class="sxs-lookup"><span data-stu-id="e9504-245">`DisablePasswordExpiration` can also be specified.</span></span> <span data-ttu-id="e9504-246">Os dois podem ser especificados juntos; por exemplo: `DisablePasswordExpiration, DisableStrongPassword`.</span><span class="sxs-lookup"><span data-stu-id="e9504-246">The two may be specified together; for example: `DisablePasswordExpiration, DisableStrongPassword`.</span></span>|
|<span data-ttu-id="e9504-247">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="e9504-247">passwordProfile</span></span>|[<span data-ttu-id="e9504-248">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="e9504-248">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="e9504-249">Especifica o perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-249">Specifies the password profile for the user.</span></span> <span data-ttu-id="e9504-250">O perfil contém a senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-250">The profile contains the user’s password.</span></span> <span data-ttu-id="e9504-251">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="e9504-251">This property is required when a user is created.</span></span> <span data-ttu-id="e9504-252">A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**.</span><span class="sxs-lookup"><span data-stu-id="e9504-252">The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property.</span></span> <span data-ttu-id="e9504-253">Por padrão, é obrigatória uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="e9504-253">By default, a strong password is required.</span></span> <span data-ttu-id="e9504-254">Isto não pode ser usado para usuários federados.</span><span class="sxs-lookup"><span data-stu-id="e9504-254">This cannot be used for federated users.</span></span> <span data-ttu-id="e9504-255">O *Diretório.AccessAsUser.All* permissão é necessária para atualizar esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="e9504-255">The *Directory.AccessAsUser.All* permission is required to update this property.</span></span>|
|<span data-ttu-id="e9504-256">pastProjects</span><span class="sxs-lookup"><span data-stu-id="e9504-256">pastProjects</span></span>|<span data-ttu-id="e9504-257">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9504-257">String collection</span></span>|<span data-ttu-id="e9504-258">Uma lista para o usuário enumerar seus projetos anteriores.</span><span class="sxs-lookup"><span data-stu-id="e9504-258">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="e9504-259">postalCode</span><span class="sxs-lookup"><span data-stu-id="e9504-259">postalCode</span></span>|<span data-ttu-id="e9504-260">String</span><span class="sxs-lookup"><span data-stu-id="e9504-260">String</span></span>|<span data-ttu-id="e9504-p122">O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.</span><span class="sxs-lookup"><span data-stu-id="e9504-p122">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="e9504-264">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="e9504-264">preferredLanguage</span></span>|<span data-ttu-id="e9504-265">String</span><span class="sxs-lookup"><span data-stu-id="e9504-265">String</span></span>|<span data-ttu-id="e9504-266">O idioma preferencial do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-266">The preferred language for the user.</span></span> <span data-ttu-id="e9504-267">Deve seguir o Código ISO 639-1; por exemplo `en-US`.</span><span class="sxs-lookup"><span data-stu-id="e9504-267">Should follow ISO 639-1 Code; for example `en-US`.</span></span>|
|<span data-ttu-id="e9504-268">responsibilities</span><span class="sxs-lookup"><span data-stu-id="e9504-268">responsibilities</span></span>|<span data-ttu-id="e9504-269">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9504-269">String collection</span></span>|<span data-ttu-id="e9504-270">Uma lista para o usuário enumerar suas responsabilidades.</span><span class="sxs-lookup"><span data-stu-id="e9504-270">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="e9504-271">schools</span><span class="sxs-lookup"><span data-stu-id="e9504-271">schools</span></span>|<span data-ttu-id="e9504-272">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9504-272">String collection</span></span>|<span data-ttu-id="e9504-273">Uma lista para o usuário enumerar as escolas que ele frequentou.</span><span class="sxs-lookup"><span data-stu-id="e9504-273">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="e9504-274">skills</span><span class="sxs-lookup"><span data-stu-id="e9504-274">skills</span></span>|<span data-ttu-id="e9504-275">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9504-275">String collection</span></span>|<span data-ttu-id="e9504-276">Uma lista para o usuário enumerar suas qualificações.</span><span class="sxs-lookup"><span data-stu-id="e9504-276">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="e9504-277">state</span><span class="sxs-lookup"><span data-stu-id="e9504-277">state</span></span>|<span data-ttu-id="e9504-278">String</span><span class="sxs-lookup"><span data-stu-id="e9504-278">String</span></span>|<span data-ttu-id="e9504-279">O estado ou município no endereço do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-279">The state or province in the user's address.</span></span>|
|<span data-ttu-id="e9504-280">streetAddress</span><span class="sxs-lookup"><span data-stu-id="e9504-280">streetAddress</span></span>|<span data-ttu-id="e9504-281">String</span><span class="sxs-lookup"><span data-stu-id="e9504-281">String</span></span>|<span data-ttu-id="e9504-282">O endereço do local de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-282">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="e9504-283">surname</span><span class="sxs-lookup"><span data-stu-id="e9504-283">surname</span></span>|<span data-ttu-id="e9504-284">String</span><span class="sxs-lookup"><span data-stu-id="e9504-284">String</span></span>|<span data-ttu-id="e9504-285">O sobrenome do usuário (nome de família ou sobrenome).</span><span class="sxs-lookup"><span data-stu-id="e9504-285">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="e9504-286">usageLocation</span><span class="sxs-lookup"><span data-stu-id="e9504-286">usageLocation</span></span>|<span data-ttu-id="e9504-287">String</span><span class="sxs-lookup"><span data-stu-id="e9504-287">String</span></span>|<span data-ttu-id="e9504-288">Um código de duas letras (padrão ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="e9504-288">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="e9504-289">Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.</span><span class="sxs-lookup"><span data-stu-id="e9504-289">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="e9504-290">Os exemplos incluem:`US`,`JP` e `GB`.</span><span class="sxs-lookup"><span data-stu-id="e9504-290">Examples include: `US`, `JP`, and `GB`.</span></span> <span data-ttu-id="e9504-291">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e9504-291">Not nullable.</span></span>|
|<span data-ttu-id="e9504-292">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9504-292">userPrincipalName</span></span>|<span data-ttu-id="e9504-293">String</span><span class="sxs-lookup"><span data-stu-id="e9504-293">String</span></span>|<span data-ttu-id="e9504-294">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-294">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="e9504-295">O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet.</span><span class="sxs-lookup"><span data-stu-id="e9504-295">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="e9504-296">Por convenção, ele deve ser mapeado para o nome de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-296">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="e9504-297">O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário.</span><span class="sxs-lookup"><span data-stu-id="e9504-297">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="e9504-298">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="e9504-298">This property is required when a user is created.</span></span> <span data-ttu-id="e9504-299">Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](../resources/organization.md).</span><span class="sxs-lookup"><span data-stu-id="e9504-299">The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md).</span></span> <span data-ttu-id="e9504-300">Oferece suporte para `$filter` e `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="e9504-300">Supports `$filter` and `$orderby`.</span></span>
|<span data-ttu-id="e9504-301">userType</span><span class="sxs-lookup"><span data-stu-id="e9504-301">userType</span></span>|<span data-ttu-id="e9504-302">String</span><span class="sxs-lookup"><span data-stu-id="e9504-302">String</span></span>|<span data-ttu-id="e9504-303">Um valor de string que pode ser usado para classificar tipos de usuário em seu diretório, como `Member` e `Guest`.</span><span class="sxs-lookup"><span data-stu-id="e9504-303">A string value that can be used to classify user types in your directory, such as `Member` and `Guest`.</span></span>          |

> [!NOTE] 
> <span data-ttu-id="e9504-304">As propriedades a seguir não podem ser atualizadas usando um contexto somente de aplicativo: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** e **skills**.</span><span class="sxs-lookup"><span data-stu-id="e9504-304">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="e9504-305">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9504-305">Response</span></span>

<span data-ttu-id="e9504-306">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e9504-306">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e9504-307">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9504-307">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="e9504-308">Exemplo 1: atualizar as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="e9504-308">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="e9504-309">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9504-309">Request</span></span>

<span data-ttu-id="e9504-310">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9504-310">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9504-311">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9504-311">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e9504-312">C#</span><span class="sxs-lookup"><span data-stu-id="e9504-312">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9504-313">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9504-313">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9504-314">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9504-314">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9504-315">Java</span><span class="sxs-lookup"><span data-stu-id="e9504-315">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e9504-316">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9504-316">Response</span></span>
<span data-ttu-id="e9504-317">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9504-317">The following example shows the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="e9504-318">Exemplo 2: atualizar as propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="e9504-318">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="e9504-319">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9504-319">Request</span></span>

<span data-ttu-id="e9504-320">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9504-320">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e9504-321">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9504-321">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e9504-322">C#</span><span class="sxs-lookup"><span data-stu-id="e9504-322">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9504-323">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9504-323">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9504-324">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9504-324">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9504-325">Java</span><span class="sxs-lookup"><span data-stu-id="e9504-325">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9504-326">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9504-326">Response</span></span>

<span data-ttu-id="e9504-327">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9504-327">The following example shows the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-3-update-the-passwordprofile-of-a-user-to-reset-their-password"></a><span data-ttu-id="e9504-328">Exemplo 3: atualizar o passwordProfile de um usuário para redefinir sua senha</span><span class="sxs-lookup"><span data-stu-id="e9504-328">Example 3: Update the passwordProfile of a user to reset their password</span></span>

<span data-ttu-id="e9504-329">O exemplo a seguir mostra uma solicitação para redefinir a senha de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e9504-329">The following example shows a request to reset the password of another user.</span></span>

#### <a name="request"></a><span data-ttu-id="e9504-330">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9504-330">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e9504-331">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9504-331">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user_passwordProfile"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "passwordProfile": {
    "forceChangePasswordNextSignIn": false,
    "password": "xWwvJ]6NMw+bWH-d"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="e9504-332">C#</span><span class="sxs-lookup"><span data-stu-id="e9504-332">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-passwordprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9504-333">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9504-333">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-passwordprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9504-334">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9504-334">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-passwordprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9504-335">Java</span><span class="sxs-lookup"><span data-stu-id="e9504-335">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-passwordprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="e9504-336">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9504-336">Response</span></span>
<!-- {
  "blockType": "response"
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
