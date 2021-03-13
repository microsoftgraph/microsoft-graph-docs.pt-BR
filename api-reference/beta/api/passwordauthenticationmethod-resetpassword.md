---
title: 'passwordAuthenticationMethod: resetPassword'
description: Redefinir a senha de um usuário
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 71f144592ec2d0d99eccbfa2d0627f74982a5fa3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761420"
---
# <a name="passwordauthenticationmethod-resetpassword"></a><span data-ttu-id="0f6aa-103">passwordAuthenticationMethod: resetPassword</span><span class="sxs-lookup"><span data-stu-id="0f6aa-103">passwordAuthenticationMethod: resetPassword</span></span>

<span data-ttu-id="0f6aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f6aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f6aa-105">Inicie uma redefinição da senha associada a um objeto de método [de autenticação de](../resources/passwordauthenticationmethod.md) senha.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-105">Initiate a reset for the password associated with a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> <span data-ttu-id="0f6aa-106">Isso só pode ser feito por um administrador com permissões apropriadas e não pode ser executado na conta de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-106">This can only be done by an administrator with appropriate permissions and cannot be performed on a user's own account.</span></span>

<span data-ttu-id="0f6aa-107">Esse fluxo grava a nova senha no Azure Active Directory e a pressiona para o Active Directory local, se configurada usando writeback de senha.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-107">This flow writes the new password to Azure Active Directory and pushes it to on-premises Active Directory if configured using password writeback.</span></span> <span data-ttu-id="0f6aa-108">O administrador pode fornecer uma nova senha ou fazer com que o sistema gere uma.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-108">The admin can either provide a new password or have the system generate one.</span></span> <span data-ttu-id="0f6aa-109">O usuário é solicitado a alterar a senha na próxima vez que entrar.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-109">The user is prompted to change their password on their next sign in.</span></span>

<span data-ttu-id="0f6aa-110">Essa redefinição é uma operação de longa duração e retornará um link no header onde o chamador pode verificar periodicamente o `Location` status da redefinição.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-110">This reset is a long-running operation and will return a link in the `Location` header where the caller can periodically check for the status of the reset.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f6aa-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f6aa-111">Permissions</span></span>

<span data-ttu-id="0f6aa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f6aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f6aa-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f6aa-114">Permission type</span></span>                        | <span data-ttu-id="0f6aa-115">Permissões agindo por si mesmo (do mínimo para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="0f6aa-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="0f6aa-116">Permissões atuando em outras pessoas (do mínimo ao mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="0f6aa-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="0f6aa-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f6aa-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f6aa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-118">Not supported.</span></span> | <span data-ttu-id="0f6aa-119">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f6aa-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="0f6aa-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f6aa-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f6aa-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-121">Not supported.</span></span> | <span data-ttu-id="0f6aa-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-122">Not supported.</span></span> |
| <span data-ttu-id="0f6aa-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f6aa-123">Application</span></span>                            | <span data-ttu-id="0f6aa-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-124">Not supported.</span></span> | <span data-ttu-id="0f6aa-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-125">Not supported.</span></span> |

<span data-ttu-id="0f6aa-126">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="0f6aa-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="0f6aa-127">Administração global</span><span class="sxs-lookup"><span data-stu-id="0f6aa-127">Global admin</span></span>
* <span data-ttu-id="0f6aa-128">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="0f6aa-128">Privileged authentication admin</span></span>
* <span data-ttu-id="0f6aa-129">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="0f6aa-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0f6aa-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f6aa-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
```

## <a name="request-headers"></a><span data-ttu-id="0f6aa-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f6aa-131">Request headers</span></span>

| <span data-ttu-id="0f6aa-132">Nome</span><span class="sxs-lookup"><span data-stu-id="0f6aa-132">Name</span></span>          | <span data-ttu-id="0f6aa-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f6aa-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0f6aa-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f6aa-134">Authorization</span></span> | <span data-ttu-id="0f6aa-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0f6aa-137">Content-type</span><span class="sxs-lookup"><span data-stu-id="0f6aa-137">Content-type</span></span>  | <span data-ttu-id="0f6aa-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f6aa-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f6aa-140">Request body</span></span>

<span data-ttu-id="0f6aa-141">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0f6aa-142">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0f6aa-142">Parameter</span></span>    | <span data-ttu-id="0f6aa-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f6aa-143">Type</span></span>        | <span data-ttu-id="0f6aa-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f6aa-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f6aa-145">newPassword</span><span class="sxs-lookup"><span data-stu-id="0f6aa-145">newPassword</span></span>|<span data-ttu-id="0f6aa-146">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0f6aa-146">String</span></span>|<span data-ttu-id="0f6aa-147">A nova senha inserida pelo administrador. Obrigatório para locatários com cenários de senha híbrida.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-147">The new password entered by the admin. Required for tenants with hybrid password scenarios.</span></span> <span data-ttu-id="0f6aa-148">Se for omitido para uma senha somente na nuvem, o sistema retornará uma senha gerada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-148">If omitted for a cloud-only password, the system returns a system-generated password.</span></span> <span data-ttu-id="0f6aa-149">Esta é uma cadeia de caracteres unicode sem outra codificação.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-149">This is a unicode string with no other encoding.</span></span> <span data-ttu-id="0f6aa-150">Ele é validado no sistema de senhas proibido do locatário antes da aceitação e deve seguir os requisitos de senha na nuvem e/ou local do locatário.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-150">It is validated against the tenant's banned password system before acceptance, and must adhere to the tenant's cloud and/or on-premises password requirements.</span></span>|

## <a name="response"></a><span data-ttu-id="0f6aa-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f6aa-151">Response</span></span>

<span data-ttu-id="0f6aa-152">Se tiver êxito, este método retornará `202 ACCEPTED` um código de resposta e uma URL no `Location` header.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-152">If successful, this method returns a `202 ACCEPTED` response code and a URL in the `Location` header.</span></span>

<span data-ttu-id="0f6aa-153">Se o chamador não enviar uma senha, uma senha gerada pela Microsoft será fornecida em um objeto JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-153">If the caller did not submit a password, a Microsoft-generated password is provided in a JSON object in the response body.</span></span>

### <a name="response-headers"></a><span data-ttu-id="0f6aa-154">Cabeçalhos de resposta</span><span class="sxs-lookup"><span data-stu-id="0f6aa-154">Response headers</span></span>

| <span data-ttu-id="0f6aa-155">Nome</span><span class="sxs-lookup"><span data-stu-id="0f6aa-155">Name</span></span>        | <span data-ttu-id="0f6aa-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f6aa-156">Description</span></span>     |
|:------------|:----------------|
|<span data-ttu-id="0f6aa-157">Local</span><span class="sxs-lookup"><span data-stu-id="0f6aa-157">Location</span></span>     | <span data-ttu-id="0f6aa-158">URL a ser chamada para verificar o status da operação.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-158">URL to call to check the status of the operation.</span></span>|
|<span data-ttu-id="0f6aa-159">Repetir-after</span><span class="sxs-lookup"><span data-stu-id="0f6aa-159">Retry-after</span></span>  | <span data-ttu-id="0f6aa-160">Duração em segundos.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-160">Duration in seconds.</span></span>|

## <a name="examples"></a><span data-ttu-id="0f6aa-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0f6aa-161">Examples</span></span>

### <a name="example-1-user-submitted-password"></a><span data-ttu-id="0f6aa-162">Exemplo 1: senha enviada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="0f6aa-162">Example 1: User-submitted password</span></span>

<span data-ttu-id="0f6aa-163">O exemplo a seguir mostra como chamar essa API quando o chamador envia uma senha.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-163">The following example shows how to call this API when the caller submits a password.</span></span>

#### <a name="request"></a><span data-ttu-id="0f6aa-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f6aa-164">Request</span></span>

<span data-ttu-id="0f6aa-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0f6aa-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f6aa-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_adminprovided"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
Content-type: application/json

{
  "newPassword": "newPassword-value",
}
```
# <a name="c"></a>[<span data-ttu-id="0f6aa-167">C#</span><span class="sxs-lookup"><span data-stu-id="0f6aa-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-adminprovided-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f6aa-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f6aa-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-adminprovided-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f6aa-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f6aa-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-adminprovided-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f6aa-170">Java</span><span class="sxs-lookup"><span data-stu-id="0f6aa-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-adminprovided-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0f6aa-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f6aa-171">Response</span></span>

<span data-ttu-id="0f6aa-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-172">The following is an example of the response.</span></span>

> <span data-ttu-id="0f6aa-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 202 ACCEPTED
Content-type: application/json
Location: https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/operations/{id}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

### <a name="example-2-system-generated-password"></a><span data-ttu-id="0f6aa-175">Exemplo 2: senha gerada pelo sistema</span><span class="sxs-lookup"><span data-stu-id="0f6aa-175">Example 2: System-generated password</span></span>

<span data-ttu-id="0f6aa-176">O exemplo a seguir mostra como chamar essa API quando o chamador não envia uma senha.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-176">The following example shows how to call this API when the caller does not submit a password.</span></span>

#### <a name="request"></a><span data-ttu-id="0f6aa-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f6aa-177">Request</span></span>

<span data-ttu-id="0f6aa-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-178">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0f6aa-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f6aa-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_systemgenerated"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
```
# <a name="c"></a>[<span data-ttu-id="0f6aa-180">C#</span><span class="sxs-lookup"><span data-stu-id="0f6aa-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-systemgenerated-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f6aa-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f6aa-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-systemgenerated-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f6aa-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f6aa-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-systemgenerated-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f6aa-183">Java</span><span class="sxs-lookup"><span data-stu-id="0f6aa-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-systemgenerated-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0f6aa-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f6aa-184">Response</span></span>

<span data-ttu-id="0f6aa-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-185">The following is an example of the response.</span></span>

> <span data-ttu-id="0f6aa-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f6aa-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/operations/{id}
Content-type: application/json

{
  "password": "new system generated password"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
