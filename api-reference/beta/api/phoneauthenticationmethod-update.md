---
title: Atualizar phoneAuthenticationMethod
description: Atualize o número de telefone associado a um objeto phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5230ca00a63f3543b95ef4f2a1dc7242c5460a1b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055404"
---
# <a name="update-phoneauthenticationmethod"></a><span data-ttu-id="42dc1-103">Atualizar phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="42dc1-103">Update phoneAuthenticationMethod</span></span>

<span data-ttu-id="42dc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42dc1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42dc1-105">Atualize o número de telefone associado a um [método de autenticação de telefone](../resources/phoneauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="42dc1-105">Update the phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span>

<span data-ttu-id="42dc1-106">Não é possível alterar o tipo de telefone.</span><span class="sxs-lookup"><span data-stu-id="42dc1-106">You can't change a phone's type.</span></span> <span data-ttu-id="42dc1-107">Para alterar o tipo de telefone, adicione um novo número do tipo desejado e exclua o objeto com o tipo original.</span><span class="sxs-lookup"><span data-stu-id="42dc1-107">To change a phone's type, add a new number of the desired type and then delete the object with the original type.</span></span>

<span data-ttu-id="42dc1-108">Se um usuário estiver habilitado pela política para usar SMS entrar e o número for alterado, o sistema tentará registrar o número para uso `mobile` nesse sistema.</span><span class="sxs-lookup"><span data-stu-id="42dc1-108">If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="42dc1-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="42dc1-109">Permissions</span></span>

<span data-ttu-id="42dc1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42dc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="42dc1-112">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="42dc1-112">Permissions acting on self</span></span>

|<span data-ttu-id="42dc1-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42dc1-113">Permission type</span></span>      | <span data-ttu-id="42dc1-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42dc1-114">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="42dc1-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42dc1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="42dc1-116">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42dc1-116">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="42dc1-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42dc1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42dc1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42dc1-118">Not supported.</span></span> |
| <span data-ttu-id="42dc1-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42dc1-119">Application</span></span>                            | <span data-ttu-id="42dc1-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42dc1-120">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="42dc1-121">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="42dc1-121">Permissions acting on other users</span></span>

|<span data-ttu-id="42dc1-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42dc1-122">Permission type</span></span>      | <span data-ttu-id="42dc1-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42dc1-123">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="42dc1-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42dc1-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="42dc1-125">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42dc1-125">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="42dc1-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42dc1-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42dc1-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42dc1-127">Not supported.</span></span> |
| <span data-ttu-id="42dc1-128">Application</span><span class="sxs-lookup"><span data-stu-id="42dc1-128">Application</span></span>                            | <span data-ttu-id="42dc1-129">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42dc1-129">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="42dc1-130">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="42dc1-130">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="42dc1-131">Administração global</span><span class="sxs-lookup"><span data-stu-id="42dc1-131">Global admin</span></span>
* <span data-ttu-id="42dc1-132">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="42dc1-132">Privileged authentication admin</span></span>
* <span data-ttu-id="42dc1-133">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="42dc1-133">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="42dc1-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42dc1-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="42dc1-135">O valor correspondente ao phoneType a `id` ser atualizado é um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="42dc1-135">The value of `id` corresponding to the phoneType to update is one of the following:</span></span>
+ <span data-ttu-id="42dc1-136">`b6332ec1-7057-4abe-9331-3d72feddfe41` para atualizar `alternateMobile` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="42dc1-136">`b6332ec1-7057-4abe-9331-3d72feddfe41` to update the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="42dc1-137">`e37fc753-ff3b-4958-9484-eaa9425c82bc` para atualizar `office` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="42dc1-137">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to update the `office` **phoneType**.</span></span>
+ <span data-ttu-id="42dc1-138">`3179e48a-750b-4051-897c-87b9720928f7` para atualizar `mobile` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="42dc1-138">`3179e48a-750b-4051-897c-87b9720928f7` to update the `mobile` **phoneType**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42dc1-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42dc1-139">Request headers</span></span>

| <span data-ttu-id="42dc1-140">Nome</span><span class="sxs-lookup"><span data-stu-id="42dc1-140">Name</span></span>       | <span data-ttu-id="42dc1-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="42dc1-141">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="42dc1-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="42dc1-142">Authorization</span></span> | <span data-ttu-id="42dc1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42dc1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42dc1-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="42dc1-145">Content-type</span></span>  | <span data-ttu-id="42dc1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42dc1-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42dc1-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42dc1-148">Request body</span></span>

<span data-ttu-id="42dc1-149">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="42dc1-149">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="42dc1-150">As propriedades existentes que não estão incluídas no corpo da solicitação serão recalculadas com base em alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="42dc1-150">Existing properties that are not included in the request body will be recalculated based on changes to other property values.</span></span>

| <span data-ttu-id="42dc1-151">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42dc1-151">Property</span></span>     | <span data-ttu-id="42dc1-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="42dc1-152">Type</span></span>        | <span data-ttu-id="42dc1-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="42dc1-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42dc1-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="42dc1-154">phoneNumber</span></span>|<span data-ttu-id="42dc1-155">String</span><span class="sxs-lookup"><span data-stu-id="42dc1-155">String</span></span>|<span data-ttu-id="42dc1-156">O número de telefone para texto ou chamada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="42dc1-156">The phone number to text or call for authentication.</span></span> <span data-ttu-id="42dc1-157">Telefone números usam o formato "+ \<country code\> \<number\> x \<extension\> ", com a extensão opcional.</span><span class="sxs-lookup"><span data-stu-id="42dc1-157">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="42dc1-158">Por exemplo, +1 5555551234 ou +1 5555551234x123 são válidos.</span><span class="sxs-lookup"><span data-stu-id="42dc1-158">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="42dc1-159">Os números são rejeitados ao criar/atualizar se não corresponderem ao formato necessário.</span><span class="sxs-lookup"><span data-stu-id="42dc1-159">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="42dc1-160">phoneType</span><span class="sxs-lookup"><span data-stu-id="42dc1-160">phoneType</span></span>|<span data-ttu-id="42dc1-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42dc1-161">string</span></span>| <span data-ttu-id="42dc1-162">Os valores possíveis são: `mobile`, `alternateMobile` ou `office`.</span><span class="sxs-lookup"><span data-stu-id="42dc1-162">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="42dc1-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="42dc1-163">Response</span></span>

<span data-ttu-id="42dc1-164">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42dc1-164">If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42dc1-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42dc1-165">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42dc1-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42dc1-166">Request</span></span>

<span data-ttu-id="42dc1-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42dc1-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42dc1-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="42dc1-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="42dc1-169">C#</span><span class="sxs-lookup"><span data-stu-id="42dc1-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42dc1-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42dc1-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42dc1-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42dc1-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42dc1-172">Java</span><span class="sxs-lookup"><span data-stu-id="42dc1-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42dc1-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="42dc1-173">Response</span></span>

<span data-ttu-id="42dc1-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42dc1-174">The following is an example of the response.</span></span>

> <span data-ttu-id="42dc1-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="42dc1-175">**Note:** The response object shown here might be shortened for readability.</span></span>

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
