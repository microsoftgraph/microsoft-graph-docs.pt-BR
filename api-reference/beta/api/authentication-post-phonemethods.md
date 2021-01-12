---
title: Criar phoneAuthenticationMethod
description: Adicione um novo método de autenticação de telefone.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 41a419425d9d4368aae34a5af0ed3c2b778165d8
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796456"
---
# <a name="create-phoneauthenticationmethod"></a><span data-ttu-id="e9dfd-103">Criar phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e9dfd-103">Create phoneAuthenticationMethod</span></span>

<span data-ttu-id="e9dfd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9dfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9dfd-105">Adicione um novo método [de autenticação de telefone.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="e9dfd-105">Add a new [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> <span data-ttu-id="e9dfd-106">Um usuário pode ter apenas um telefone de cada tipo, capturado na **propriedade phoneType.**</span><span class="sxs-lookup"><span data-stu-id="e9dfd-106">A user may only have one phone of each type, captured in the **phoneType** property.</span></span> <span data-ttu-id="e9dfd-107">Isso significa que, por exemplo, a adição de um telefone a um usuário com um telefone `mobile` `mobile` pré-clássico falhará.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-107">This means, for example, adding a `mobile` phone to a user with a preexisting `mobile` phone will fail.</span></span> <span data-ttu-id="e9dfd-108">Além disso, um usuário sempre deve ter `mobile` um telefone antes de adicionar um `alternateMobile` telefone.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-108">Additionally, a user must always have a `mobile` phone before adding an `alternateMobile` phone.</span></span>

<span data-ttu-id="e9dfd-109">A adição de um número de telefone o disponibiliza para uso na autenticação multifatória do Azure (MFA) e na redefinição de senha de autoatendado (SSPR), se habilitada.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-109">Adding a phone number makes it available for use in both Azure multi-factor authentication (MFA) and self-service password reset (SSPR), if enabled.</span></span>

<span data-ttu-id="e9dfd-110">Além disso, se um usuário for habilitado pela política para usar a inscrição em SMS e um número for adicionado, o sistema tentará registrar o número para uso `mobile` no sistema.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-110">Additionally, if a user is enabled by policy to use SMS sign-in and a `mobile` number is added, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9dfd-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e9dfd-111">Permissions</span></span>

<span data-ttu-id="e9dfd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9dfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9dfd-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9dfd-114">Permission type</span></span>                        | <span data-ttu-id="e9dfd-115">Permissões atuando por si mesmo (do menos para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="e9dfd-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="e9dfd-116">Permissões atuando em outras pessoas (de menos para mais privilegiados)</span><span class="sxs-lookup"><span data-stu-id="e9dfd-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="e9dfd-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9dfd-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9dfd-118">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9dfd-118">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="e9dfd-119">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9dfd-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="e9dfd-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9dfd-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9dfd-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-121">Not supported.</span></span> | <span data-ttu-id="e9dfd-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-122">Not supported.</span></span> |
| <span data-ttu-id="e9dfd-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9dfd-123">Application</span></span>                            | <span data-ttu-id="e9dfd-124">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-124">Not applicable.</span></span> | <span data-ttu-id="e9dfd-125">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9dfd-125">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="e9dfd-126">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="e9dfd-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="e9dfd-127">Administração global</span><span class="sxs-lookup"><span data-stu-id="e9dfd-127">Global admin</span></span>
* <span data-ttu-id="e9dfd-128">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="e9dfd-128">Privileged authentication admin</span></span>
* <span data-ttu-id="e9dfd-129">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="e9dfd-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="e9dfd-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9dfd-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="request-headers"></a><span data-ttu-id="e9dfd-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9dfd-131">Request headers</span></span>

| <span data-ttu-id="e9dfd-132">Nome</span><span class="sxs-lookup"><span data-stu-id="e9dfd-132">Name</span></span>          | <span data-ttu-id="e9dfd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9dfd-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e9dfd-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9dfd-134">Authorization</span></span> | <span data-ttu-id="e9dfd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9dfd-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9dfd-137">Content-Type</span></span>  | <span data-ttu-id="e9dfd-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9dfd-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9dfd-140">Request body</span></span>

<span data-ttu-id="e9dfd-141">No corpo da solicitação, fornece uma representação JSON de um [objeto phoneAuthenticationMethod.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="e9dfd-141">In the request body, supply a JSON representation of a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span> <span data-ttu-id="e9dfd-142">O JSON deve `phoneNumber` incluir `phoneType` e, mas não `smsSignInState` (que é somente leitura).</span><span class="sxs-lookup"><span data-stu-id="e9dfd-142">The JSON must include `phoneNumber` and `phoneType`, but not `smsSignInState` (which is read-only).</span></span>

| <span data-ttu-id="e9dfd-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9dfd-143">Property</span></span>     | <span data-ttu-id="e9dfd-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9dfd-144">Type</span></span>        | <span data-ttu-id="e9dfd-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9dfd-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9dfd-146">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="e9dfd-146">phoneNumber</span></span>|<span data-ttu-id="e9dfd-147">String</span><span class="sxs-lookup"><span data-stu-id="e9dfd-147">String</span></span>|<span data-ttu-id="e9dfd-148">O número de telefone para texto ou chamada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-148">The phone number to text or call for authentication.</span></span> <span data-ttu-id="e9dfd-149">Os números de telefone usam o formato "+ \<country code\> \<number\> \<extension\> x", com extensão opcional.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-149">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="e9dfd-150">Por exemplo, +1 5555551234 ou +1 5555551234x123 são válidos.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-150">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="e9dfd-151">Os números serão rejeitados ao criar/atualizar se não corresponderem ao formato necessário.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-151">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="e9dfd-152">phoneType</span><span class="sxs-lookup"><span data-stu-id="e9dfd-152">phoneType</span></span>|<span data-ttu-id="e9dfd-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9dfd-153">String</span></span>|<span data-ttu-id="e9dfd-154">Os valores possíveis `mobile` são: `alternateMobile` , e `office` .</span><span class="sxs-lookup"><span data-stu-id="e9dfd-154">Possible values are: `mobile`, `alternateMobile`, and `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="e9dfd-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9dfd-155">Response</span></span>

<span data-ttu-id="e9dfd-156">Se bem-sucedido, este método retorna um código de resposta e um novo `201 Created` [objeto phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-156">If successful, this method returns a `201 Created` response code and a new [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9dfd-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e9dfd-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9dfd-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9dfd-158">Request</span></span>

<span data-ttu-id="e9dfd-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9dfd-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9dfd-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e9dfd-161">C#</span><span class="sxs-lookup"><span data-stu-id="e9dfd-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-phoneauthenticationmethod-from-authentication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9dfd-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9dfd-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-phoneauthenticationmethod-from-authentication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9dfd-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9dfd-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-phoneauthenticationmethod-from-authentication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9dfd-164">Java</span><span class="sxs-lookup"><span data-stu-id="e9dfd-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-phoneauthenticationmethod-from-authentication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9dfd-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9dfd-165">Response</span></span>

<span data-ttu-id="e9dfd-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-166">The following is an example of the response.</span></span>

> <span data-ttu-id="e9dfd-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9dfd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
