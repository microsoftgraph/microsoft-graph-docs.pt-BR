---
title: Atualizar phoneAuthenticationMethod
description: Atualize o número de telefone associado ao objeto phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a565fac12b24b21dd43d87b4a736971bccf79115
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980515"
---
# <a name="update-phoneauthenticationmethod"></a><span data-ttu-id="9f6c8-103">Atualizar phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9f6c8-103">Update phoneAuthenticationMethod</span></span>

<span data-ttu-id="9f6c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f6c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f6c8-105">Atualize o número de telefone associado a um [método de autenticação de telefone](../resources/phoneauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="9f6c8-105">Update the phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span>

<span data-ttu-id="9f6c8-106">Não é possível alterar o tipo de um telefone.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-106">You can't change a phone's type.</span></span> <span data-ttu-id="9f6c8-107">Para alterar o tipo de um telefone, adicione um novo número do tipo desejado e exclua o objeto com o tipo original.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-107">To change a phone's type, add a new number of the desired type and then delete the object with the original type.</span></span>

<span data-ttu-id="9f6c8-108">Se um usuário estiver habilitado por política para usar o SMS para entrar e o `mobile` número for alterado, o sistema tentará registrar o número para uso nesse sistema.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-108">If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f6c8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f6c8-109">Permissions</span></span>

<span data-ttu-id="9f6c8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f6c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f6c8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f6c8-112">Permission type</span></span>                        | <span data-ttu-id="9f6c8-113">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f6c8-113">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="9f6c8-114">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f6c8-114">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="9f6c8-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f6c8-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f6c8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-116">Not supported.</span></span> | <span data-ttu-id="9f6c8-117">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9f6c8-117">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9f6c8-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f6c8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f6c8-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-119">Not supported.</span></span> | <span data-ttu-id="9f6c8-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-120">Not supported.</span></span> |
| <span data-ttu-id="9f6c8-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f6c8-121">Application</span></span>                            | <span data-ttu-id="9f6c8-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-122">Not supported.</span></span> | <span data-ttu-id="9f6c8-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-123">Not supported.</span></span> |

<span data-ttu-id="9f6c8-124">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="9f6c8-124">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="9f6c8-125">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9f6c8-125">Global admin</span></span>
* <span data-ttu-id="9f6c8-126">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="9f6c8-126">Privileged authentication admin</span></span>
* <span data-ttu-id="9f6c8-127">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="9f6c8-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9f6c8-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f6c8-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f6c8-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f6c8-129">Request headers</span></span>

| <span data-ttu-id="9f6c8-130">Nome</span><span class="sxs-lookup"><span data-stu-id="9f6c8-130">Name</span></span>       | <span data-ttu-id="9f6c8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f6c8-131">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9f6c8-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f6c8-132">Authorization</span></span> | <span data-ttu-id="9f6c8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f6c8-135">Content-type</span><span class="sxs-lookup"><span data-stu-id="9f6c8-135">Content-type</span></span>  | <span data-ttu-id="9f6c8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f6c8-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f6c8-138">Request body</span></span>

<span data-ttu-id="9f6c8-139">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-139">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9f6c8-140">As propriedades existentes que não estão incluídas no corpo da solicitação serão recalculadas com base nas alterações de outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-140">Existing properties that are not included in the request body will be recalculated based on changes to other property values.</span></span>

| <span data-ttu-id="9f6c8-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f6c8-141">Property</span></span>     | <span data-ttu-id="9f6c8-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f6c8-142">Type</span></span>        | <span data-ttu-id="9f6c8-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f6c8-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9f6c8-144">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="9f6c8-144">phoneNumber</span></span>|<span data-ttu-id="9f6c8-145">String</span><span class="sxs-lookup"><span data-stu-id="9f6c8-145">String</span></span>|<span data-ttu-id="9f6c8-146">O número de telefone para texto ou chamada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-146">The phone number to text or call for authentication.</span></span> <span data-ttu-id="9f6c8-147">Os números de telefone usam o formato "+ \<country code\> \<number\> x \<extension\> ", com a extensão opcional.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-147">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="9f6c8-148">Por exemplo, + 1 5555551234 ou + 1 5555551234x123 são válidas.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-148">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="9f6c8-149">Os números são rejeitados ao criar/atualizar se não coincidem com o formato necessário.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-149">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="9f6c8-150">PhoneType</span><span class="sxs-lookup"><span data-stu-id="9f6c8-150">phoneType</span></span>|<span data-ttu-id="9f6c8-151">string</span><span class="sxs-lookup"><span data-stu-id="9f6c8-151">string</span></span>| <span data-ttu-id="9f6c8-152">Os valores possíveis são: `mobile` , `alternateMobile` , ou `office` .</span><span class="sxs-lookup"><span data-stu-id="9f6c8-152">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="9f6c8-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f6c8-153">Response</span></span>

<span data-ttu-id="9f6c8-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-154">If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f6c8-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9f6c8-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f6c8-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f6c8-156">Request</span></span>

<span data-ttu-id="9f6c8-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f6c8-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f6c8-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9f6c8-159">C#</span><span class="sxs-lookup"><span data-stu-id="9f6c8-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f6c8-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f6c8-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f6c8-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f6c8-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f6c8-162">Java</span><span class="sxs-lookup"><span data-stu-id="9f6c8-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9f6c8-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f6c8-163">Response</span></span>

<span data-ttu-id="9f6c8-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-164">The following is an example of the response.</span></span>

> <span data-ttu-id="9f6c8-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f6c8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
