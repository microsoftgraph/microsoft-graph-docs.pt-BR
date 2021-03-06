---
title: Atualizar phoneAuthenticationMethod
description: Atualize o número de telefone associado a um objeto phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: af68131407948d1986a74e6f6d97540891f617b4
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516805"
---
# <a name="update-phoneauthenticationmethod"></a><span data-ttu-id="92c53-103">Atualizar phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="92c53-103">Update phoneAuthenticationMethod</span></span>

<span data-ttu-id="92c53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92c53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92c53-105">Atualize o número de telefone associado a um [método de autenticação de telefone](../resources/phoneauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="92c53-105">Update the phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span>

<span data-ttu-id="92c53-106">Não é possível alterar o tipo de telefone.</span><span class="sxs-lookup"><span data-stu-id="92c53-106">You can't change a phone's type.</span></span> <span data-ttu-id="92c53-107">Para alterar o tipo de telefone, adicione um novo número do tipo desejado e exclua o objeto com o tipo original.</span><span class="sxs-lookup"><span data-stu-id="92c53-107">To change a phone's type, add a new number of the desired type and then delete the object with the original type.</span></span>

<span data-ttu-id="92c53-108">Se um usuário estiver habilitado pela política para usar o SMS para entrar e o número for alterado, o sistema tentará registrar o número para `mobile` uso nesse sistema.</span><span class="sxs-lookup"><span data-stu-id="92c53-108">If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="92c53-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="92c53-109">Permissions</span></span>

<span data-ttu-id="92c53-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92c53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="92c53-112">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="92c53-112">Permissions acting on self</span></span>

|<span data-ttu-id="92c53-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92c53-113">Permission type</span></span>      | <span data-ttu-id="92c53-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92c53-114">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="92c53-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92c53-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="92c53-116">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c53-116">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="92c53-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92c53-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92c53-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92c53-118">Not supported.</span></span> |
| <span data-ttu-id="92c53-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92c53-119">Application</span></span>                            | <span data-ttu-id="92c53-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92c53-120">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="92c53-121">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="92c53-121">Permissions acting on other users</span></span>

|<span data-ttu-id="92c53-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92c53-122">Permission type</span></span>      | <span data-ttu-id="92c53-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92c53-123">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="92c53-124">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92c53-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="92c53-125">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92c53-125">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="92c53-126">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92c53-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92c53-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92c53-127">Not supported.</span></span> |
| <span data-ttu-id="92c53-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92c53-128">Application</span></span>                            | <span data-ttu-id="92c53-129">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92c53-129">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="92c53-130">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="92c53-130">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="92c53-131">Administrador global</span><span class="sxs-lookup"><span data-stu-id="92c53-131">Global admin</span></span>
* <span data-ttu-id="92c53-132">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="92c53-132">Privileged authentication admin</span></span>
* <span data-ttu-id="92c53-133">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="92c53-133">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="92c53-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92c53-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92c53-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92c53-135">Request headers</span></span>

| <span data-ttu-id="92c53-136">Nome</span><span class="sxs-lookup"><span data-stu-id="92c53-136">Name</span></span>       | <span data-ttu-id="92c53-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="92c53-137">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="92c53-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="92c53-138">Authorization</span></span> | <span data-ttu-id="92c53-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92c53-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92c53-141">Content-type</span><span class="sxs-lookup"><span data-stu-id="92c53-141">Content-type</span></span>  | <span data-ttu-id="92c53-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92c53-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92c53-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92c53-144">Request body</span></span>

<span data-ttu-id="92c53-145">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="92c53-145">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="92c53-146">As propriedades existentes que não estão incluídas no corpo da solicitação serão recalculadas com base em alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="92c53-146">Existing properties that are not included in the request body will be recalculated based on changes to other property values.</span></span>

| <span data-ttu-id="92c53-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92c53-147">Property</span></span>     | <span data-ttu-id="92c53-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="92c53-148">Type</span></span>        | <span data-ttu-id="92c53-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="92c53-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="92c53-150">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="92c53-150">phoneNumber</span></span>|<span data-ttu-id="92c53-151">String</span><span class="sxs-lookup"><span data-stu-id="92c53-151">String</span></span>|<span data-ttu-id="92c53-152">O número de telefone para texto ou chamada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="92c53-152">The phone number to text or call for authentication.</span></span> <span data-ttu-id="92c53-153">Os números de telefone usam o formato "+ \<country code\> \<number\> \<extension\> x", com a extensão opcional.</span><span class="sxs-lookup"><span data-stu-id="92c53-153">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="92c53-154">Por exemplo, +1 5555551234 ou +1 5555551234x123 são válidos.</span><span class="sxs-lookup"><span data-stu-id="92c53-154">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="92c53-155">Os números são rejeitados ao criar/atualizar se não corresponderem ao formato necessário.</span><span class="sxs-lookup"><span data-stu-id="92c53-155">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="92c53-156">phoneType</span><span class="sxs-lookup"><span data-stu-id="92c53-156">phoneType</span></span>|<span data-ttu-id="92c53-157">string</span><span class="sxs-lookup"><span data-stu-id="92c53-157">string</span></span>| <span data-ttu-id="92c53-158">Os valores possíveis são: `mobile`, `alternateMobile` ou `office`.</span><span class="sxs-lookup"><span data-stu-id="92c53-158">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="92c53-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="92c53-159">Response</span></span>

<span data-ttu-id="92c53-160">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92c53-160">If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92c53-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="92c53-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="92c53-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92c53-162">Request</span></span>

<span data-ttu-id="92c53-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92c53-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92c53-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="92c53-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_phoneauthenticationmethod"
}-->

```http
PUT https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
}
```
# <a name="c"></a>[<span data-ttu-id="92c53-165">C#</span><span class="sxs-lookup"><span data-stu-id="92c53-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92c53-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92c53-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92c53-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92c53-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92c53-168">Java</span><span class="sxs-lookup"><span data-stu-id="92c53-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="92c53-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="92c53-169">Response</span></span>

<span data-ttu-id="92c53-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92c53-170">The following is an example of the response.</span></span>

> <span data-ttu-id="92c53-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92c53-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update phoneauthenticationmethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
