---
title: 'passwordAuthenticationMethod: resetPassword'
description: Redefinir a senha de um usuário
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9dabb63709b42f7eaa9c3791e9e91300f5063469
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805978"
---
# <a name="passwordauthenticationmethod-resetpassword"></a><span data-ttu-id="779a6-103">passwordAuthenticationMethod: resetPassword</span><span class="sxs-lookup"><span data-stu-id="779a6-103">passwordAuthenticationMethod: resetPassword</span></span>

<span data-ttu-id="779a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="779a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="779a6-105">Inicie uma redefinição para a senha associada a um objeto de [método de autenticação de senha](../resources/passwordauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="779a6-105">Initiate a reset for the password associated with a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> <span data-ttu-id="779a6-106">Isso só pode ser feito por um administrador com as permissões apropriadas e não pode ser executado na conta de um usuário.</span><span class="sxs-lookup"><span data-stu-id="779a6-106">This can only be done by an administrator with appropriate permissions and cannot be performed on a user's own account.</span></span>

<span data-ttu-id="779a6-107">Este fluxo grava a nova senha no Azure Active Directory e a envia para o Active Directory local, se configurado usando o Write-back de senha.</span><span class="sxs-lookup"><span data-stu-id="779a6-107">This flow writes the new password to Azure Active Directory and pushes it to on-premises Active Directory if configured using password writeback.</span></span> <span data-ttu-id="779a6-108">O administrador pode fornecer uma nova senha ou fazer com que o sistema gere uma.</span><span class="sxs-lookup"><span data-stu-id="779a6-108">The admin can either provide a new password or have the system generate one.</span></span> <span data-ttu-id="779a6-109">O usuário é solicitado a alterar a senha na próxima vez em que entrar.</span><span class="sxs-lookup"><span data-stu-id="779a6-109">The user is prompted to change their password on their next sign in.</span></span>

<span data-ttu-id="779a6-110">Essa redefinição é uma operação de execução longa e retornará um link no `Location` cabeçalho onde o chamador pode verificar periodicamente o status da redefinição.</span><span class="sxs-lookup"><span data-stu-id="779a6-110">This reset is a long-running operation and will return a link in the `Location` header where the caller can periodically check for the status of the reset.</span></span>

## <a name="permissions"></a><span data-ttu-id="779a6-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="779a6-111">Permissions</span></span>

<span data-ttu-id="779a6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="779a6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="779a6-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="779a6-114">Permission type</span></span>                        | <span data-ttu-id="779a6-115">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="779a6-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="779a6-116">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="779a6-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="779a6-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="779a6-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="779a6-118">UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="779a6-118">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="779a6-119">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="779a6-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="779a6-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="779a6-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="779a6-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="779a6-121">Not supported.</span></span> | <span data-ttu-id="779a6-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="779a6-122">Not supported.</span></span> |
| <span data-ttu-id="779a6-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="779a6-123">Application</span></span>                            | <span data-ttu-id="779a6-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="779a6-124">Not supported.</span></span> | <span data-ttu-id="779a6-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="779a6-125">Not supported.</span></span> |

<span data-ttu-id="779a6-126">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="779a6-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="779a6-127">Administrador global</span><span class="sxs-lookup"><span data-stu-id="779a6-127">Global admin</span></span>
* <span data-ttu-id="779a6-128">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="779a6-128">Privileged authentication admin</span></span>
* <span data-ttu-id="779a6-129">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="779a6-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="779a6-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="779a6-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id}/authentication/passwordMethods/{id}/resetPassword
```

## <a name="request-headers"></a><span data-ttu-id="779a6-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="779a6-131">Request headers</span></span>

| <span data-ttu-id="779a6-132">Nome</span><span class="sxs-lookup"><span data-stu-id="779a6-132">Name</span></span>          | <span data-ttu-id="779a6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="779a6-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="779a6-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="779a6-134">Authorization</span></span> | <span data-ttu-id="779a6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="779a6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="779a6-137">Content-type</span><span class="sxs-lookup"><span data-stu-id="779a6-137">Content-type</span></span>  | <span data-ttu-id="779a6-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="779a6-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="779a6-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="779a6-140">Request body</span></span>

<span data-ttu-id="779a6-141">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="779a6-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="779a6-142">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="779a6-142">Parameter</span></span>    | <span data-ttu-id="779a6-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="779a6-143">Type</span></span>        | <span data-ttu-id="779a6-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="779a6-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="779a6-145">newPassword</span><span class="sxs-lookup"><span data-stu-id="779a6-145">newPassword</span></span>|<span data-ttu-id="779a6-146">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="779a6-146">String</span></span>|<span data-ttu-id="779a6-147">A nova senha inserida pelo administrador. Obrigatório para locatários com cenários de senha híbrida.</span><span class="sxs-lookup"><span data-stu-id="779a6-147">The new password entered by the admin. Required for tenants with hybrid password scenarios.</span></span> <span data-ttu-id="779a6-148">Se for omitido para uma senha somente de nuvem, o sistema retornará uma senha gerada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="779a6-148">If omitted for a cloud-only password, the system returns a system-generated password.</span></span> <span data-ttu-id="779a6-149">Esta é uma cadeia de caracteres Unicode sem codificação.</span><span class="sxs-lookup"><span data-stu-id="779a6-149">This is a unicode string with no other encoding.</span></span> <span data-ttu-id="779a6-150">Ele é validado em relação ao sistema de senha banida do locatário antes da aceitação e deve cumprir a nuvem do locatário e/ou os requisitos de senha local.</span><span class="sxs-lookup"><span data-stu-id="779a6-150">It is validated against the tenant's banned password system before acceptance, and must adhere to the tenant's cloud and/or on-premises password requirements.</span></span>|

## <a name="response"></a><span data-ttu-id="779a6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="779a6-151">Response</span></span>

<span data-ttu-id="779a6-152">Se tiver êxito, este método retornará `202 ACCEPTED` um código de resposta e uma URL `Location` no cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="779a6-152">If successful, this method returns a `202 ACCEPTED` response code and a URL in the `Location` header.</span></span>

<span data-ttu-id="779a6-153">Se o chamador não enviar uma senha, uma senha gerada pela Microsoft será fornecida em um objeto JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="779a6-153">If the caller did not submit a password, a Microsoft-generated password is provided in a JSON object in the response body.</span></span>

### <a name="response-headers"></a><span data-ttu-id="779a6-154">Cabeçalhos de resposta</span><span class="sxs-lookup"><span data-stu-id="779a6-154">Response headers</span></span>

| <span data-ttu-id="779a6-155">Nome</span><span class="sxs-lookup"><span data-stu-id="779a6-155">Name</span></span>        | <span data-ttu-id="779a6-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="779a6-156">Description</span></span>     |
|:------------|:----------------|
|<span data-ttu-id="779a6-157">Local</span><span class="sxs-lookup"><span data-stu-id="779a6-157">Location</span></span>     | <span data-ttu-id="779a6-158">URL a ser chamada para verificar o status da operação.</span><span class="sxs-lookup"><span data-stu-id="779a6-158">URL to call to check the status of the operation.</span></span>|
|<span data-ttu-id="779a6-159">Repetir-após</span><span class="sxs-lookup"><span data-stu-id="779a6-159">Retry-after</span></span>  | <span data-ttu-id="779a6-160">Duração em segundos.</span><span class="sxs-lookup"><span data-stu-id="779a6-160">Duration in seconds.</span></span>|

## <a name="examples"></a><span data-ttu-id="779a6-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="779a6-161">Examples</span></span>

### <a name="example-1-user-submitted-password"></a><span data-ttu-id="779a6-162">Exemplo 1: senha enviada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="779a6-162">Example 1: User-submitted password</span></span>

<span data-ttu-id="779a6-163">O exemplo a seguir mostra como chamar essa API quando o chamador enviar uma senha.</span><span class="sxs-lookup"><span data-stu-id="779a6-163">The following example shows how to call this API when the caller submits a password.</span></span>

#### <a name="request"></a><span data-ttu-id="779a6-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="779a6-164">Request</span></span>

<span data-ttu-id="779a6-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="779a6-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="779a6-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="779a6-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_adminprovided"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/authentication/passwordMethods/{id}/resetPassword
Content-type: application/json

{
  "newPassword": "newPassword-value",
}
```
# <a name="c"></a>[<span data-ttu-id="779a6-167">C#</span><span class="sxs-lookup"><span data-stu-id="779a6-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-adminprovided-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="779a6-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="779a6-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-adminprovided-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="779a6-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="779a6-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-adminprovided-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="779a6-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="779a6-170">Response</span></span>

<span data-ttu-id="779a6-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="779a6-171">The following is an example of the response.</span></span>

> <span data-ttu-id="779a6-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="779a6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 202 ACCEPTED
Content-type: application/json
Location: https://graph.microsoft.com/beta/users/{id}/authentication/operations/{id}
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

### <a name="example-2-system-generated-password"></a><span data-ttu-id="779a6-174">Exemplo 2: senha gerada pelo sistema</span><span class="sxs-lookup"><span data-stu-id="779a6-174">Example 2: System-generated password</span></span>

<span data-ttu-id="779a6-175">O exemplo a seguir mostra como chamar essa API quando o chamador não enviar uma senha.</span><span class="sxs-lookup"><span data-stu-id="779a6-175">The following example shows how to call this API when the caller does not submit a password.</span></span>

#### <a name="request"></a><span data-ttu-id="779a6-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="779a6-176">Request</span></span>

<span data-ttu-id="779a6-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="779a6-177">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="779a6-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="779a6-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_systemgenerated"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/authentication/passwordMethods/{id}/resetPassword
```
# <a name="c"></a>[<span data-ttu-id="779a6-179">C#</span><span class="sxs-lookup"><span data-stu-id="779a6-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-systemgenerated-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="779a6-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="779a6-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-systemgenerated-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="779a6-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="779a6-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-systemgenerated-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="779a6-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="779a6-182">Response</span></span>

<span data-ttu-id="779a6-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="779a6-183">The following is an example of the response.</span></span>

> <span data-ttu-id="779a6-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="779a6-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/users/{id}/authentication/operations/{id}
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
