---
title: Criar phoneAuthenticationMethod
description: Adicione um novo método de autenticação de telefone.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6ebed72ef48e116273994d85f60abced79d862db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991639"
---
# <a name="create-phoneauthenticationmethod"></a><span data-ttu-id="eebef-103">Criar phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="eebef-103">Create phoneAuthenticationMethod</span></span>

<span data-ttu-id="eebef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eebef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eebef-105">Adicione um novo [método de autenticação de telefone](../resources/phoneauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="eebef-105">Add a new [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> <span data-ttu-id="eebef-106">Um usuário pode ter apenas um telefone de cada tipo, capturado na propriedade **PhoneType** .</span><span class="sxs-lookup"><span data-stu-id="eebef-106">A user may only have one phone of each type, captured in the **phoneType** property.</span></span> <span data-ttu-id="eebef-107">Isso significa que, por exemplo, adicionar um `mobile` telefone a um usuário com um telefone preexistente `mobile` falhará.</span><span class="sxs-lookup"><span data-stu-id="eebef-107">This means, for example, adding a `mobile` phone to a user with a preexisting `mobile` phone will fail.</span></span> <span data-ttu-id="eebef-108">Além disso, um usuário deve sempre ter um `mobile` telefone antes de adicionar um `alternateMobile` telefone.</span><span class="sxs-lookup"><span data-stu-id="eebef-108">Additionally, a user must always have a `mobile` phone before adding an `alternateMobile` phone.</span></span>

<span data-ttu-id="eebef-109">Adicionar um número de telefone o torna disponível para uso na autenticação multifator do Azure (MFA) e redefinição de senha de autoatendimento (SSPR), se habilitada.</span><span class="sxs-lookup"><span data-stu-id="eebef-109">Adding a phone number makes it available for use in both Azure multi-factor authentication (MFA) and self-service password reset (SSPR), if enabled.</span></span>

<span data-ttu-id="eebef-110">Além disso, se um usuário estiver habilitado por política para usar a entrada do SMS e um `mobile` número for adicionado, o sistema tentará registrar o número para uso nesse sistema.</span><span class="sxs-lookup"><span data-stu-id="eebef-110">Additionally, if a user is enabled by policy to use SMS sign-in and a `mobile` number is added, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="eebef-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="eebef-111">Permissions</span></span>

<span data-ttu-id="eebef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eebef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eebef-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eebef-114">Permission type</span></span>                        | <span data-ttu-id="eebef-115">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eebef-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="eebef-116">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eebef-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="eebef-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eebef-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="eebef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eebef-118">Not supported.</span></span> | <span data-ttu-id="eebef-119">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eebef-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="eebef-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eebef-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eebef-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eebef-121">Not supported.</span></span> | <span data-ttu-id="eebef-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eebef-122">Not supported.</span></span> |
| <span data-ttu-id="eebef-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eebef-123">Application</span></span>                            | <span data-ttu-id="eebef-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eebef-124">Not supported.</span></span> | <span data-ttu-id="eebef-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eebef-125">Not supported.</span></span> |

<span data-ttu-id="eebef-126">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="eebef-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="eebef-127">Administrador global</span><span class="sxs-lookup"><span data-stu-id="eebef-127">Global admin</span></span>
* <span data-ttu-id="eebef-128">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="eebef-128">Privileged authentication admin</span></span>
* <span data-ttu-id="eebef-129">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="eebef-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="eebef-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eebef-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id}/authentication/phoneMethods
```

## <a name="request-headers"></a><span data-ttu-id="eebef-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eebef-131">Request headers</span></span>

| <span data-ttu-id="eebef-132">Nome</span><span class="sxs-lookup"><span data-stu-id="eebef-132">Name</span></span>          | <span data-ttu-id="eebef-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eebef-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="eebef-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="eebef-134">Authorization</span></span> | <span data-ttu-id="eebef-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eebef-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eebef-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eebef-137">Content-Type</span></span>  | <span data-ttu-id="eebef-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eebef-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eebef-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eebef-140">Request body</span></span>

<span data-ttu-id="eebef-141">No corpo da solicitação, forneça uma representação JSON de um objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="eebef-141">In the request body, supply a JSON representation of a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span> <span data-ttu-id="eebef-142">O JSON deve incluir `phoneNumber` e `phoneType` , mas não `smsSignInState` (que é somente leitura).</span><span class="sxs-lookup"><span data-stu-id="eebef-142">The JSON must include `phoneNumber` and `phoneType`, but not `smsSignInState` (which is read-only).</span></span>

| <span data-ttu-id="eebef-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eebef-143">Property</span></span>     | <span data-ttu-id="eebef-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="eebef-144">Type</span></span>        | <span data-ttu-id="eebef-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="eebef-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eebef-146">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="eebef-146">phoneNumber</span></span>|<span data-ttu-id="eebef-147">String</span><span class="sxs-lookup"><span data-stu-id="eebef-147">String</span></span>|<span data-ttu-id="eebef-148">O número de telefone para texto ou chamada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="eebef-148">The phone number to text or call for authentication.</span></span> <span data-ttu-id="eebef-149">Os números de telefone usam o formato "+ \<country code\> \<number\> x \<extension\> ", com a extensão opcional.</span><span class="sxs-lookup"><span data-stu-id="eebef-149">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="eebef-150">Por exemplo, + 1 5555551234 ou + 1 5555551234x123 são válidas.</span><span class="sxs-lookup"><span data-stu-id="eebef-150">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="eebef-151">Os números são rejeitados ao criar/atualizar se não coincidem com o formato necessário.</span><span class="sxs-lookup"><span data-stu-id="eebef-151">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="eebef-152">PhoneType</span><span class="sxs-lookup"><span data-stu-id="eebef-152">phoneType</span></span>|<span data-ttu-id="eebef-153">String</span><span class="sxs-lookup"><span data-stu-id="eebef-153">String</span></span>|<span data-ttu-id="eebef-154">Os valores possíveis são: `mobile` , `alternateMobile` , e `office` .</span><span class="sxs-lookup"><span data-stu-id="eebef-154">Possible values are: `mobile`, `alternateMobile`, and `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="eebef-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="eebef-155">Response</span></span>

<span data-ttu-id="eebef-156">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eebef-156">If successful, this method returns a `201 Created` response code and a new [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eebef-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eebef-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eebef-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eebef-158">Request</span></span>

<span data-ttu-id="eebef-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eebef-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eebef-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="eebef-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_phoneauthenticationmethod_from_authentication"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile"
}
```
# <a name="c"></a>[<span data-ttu-id="eebef-161">C#</span><span class="sxs-lookup"><span data-stu-id="eebef-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-phoneauthenticationmethod-from-authentication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eebef-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eebef-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-phoneauthenticationmethod-from-authentication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eebef-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eebef-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-phoneauthenticationmethod-from-authentication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eebef-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="eebef-164">Response</span></span>

<span data-ttu-id="eebef-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eebef-165">The following is an example of the response.</span></span>

> <span data-ttu-id="eebef-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eebef-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "phoneType-value",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


