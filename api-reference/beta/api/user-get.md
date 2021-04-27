---
title: Obter um usuário
description: Recuperar as propriedades e os relacionamentos do objeto user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8a71a50714d18d4d4d8e91a4f5a7e0c0b31fe9e6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052632"
---
# <a name="get-a-user"></a><span data-ttu-id="0728d-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="0728d-103">Get a user</span></span>

<span data-ttu-id="0728d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0728d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0728d-105">Recuperar as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="0728d-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="0728d-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="0728d-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="0728d-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="0728d-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="0728d-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](user-get.md) para o usuário e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="0728d-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="0728d-109">Como o recurso **usuário** dá suporte a [extensões](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **usuário**.</span><span class="sxs-lookup"><span data-stu-id="0728d-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="0728d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0728d-110">Permissions</span></span>
<span data-ttu-id="0728d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0728d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0728d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0728d-113">Permission type</span></span>      | <span data-ttu-id="0728d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0728d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0728d-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0728d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0728d-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0728d-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0728d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0728d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0728d-118">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0728d-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="0728d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0728d-119">Application</span></span> | <span data-ttu-id="0728d-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0728d-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="0728d-121">Chamar o ponto de extremidade `/me` exige um usuário conectado e, portanto, uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="0728d-121">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="0728d-122">Não há suporte para permissões do aplicativo ao usar o ponto de extremidade `/me`.</span><span class="sxs-lookup"><span data-stu-id="0728d-122">Application permissions are not supported when using the `/me` endpoint.</span></span>

<span data-ttu-id="0728d-123">Para um usuário específico:</span><span class="sxs-lookup"><span data-stu-id="0728d-123">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="0728d-124">Observe que quando **userPrincipalName** começar com um caractere `$`, remova a barra (/) logo após `/users` e coloque **userPrincipalName** entre parênteses e aspas simples.</span><span class="sxs-lookup"><span data-stu-id="0728d-124">Note that when the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes.</span></span> <span data-ttu-id="0728d-125">Para saber mais, consulte a lista [problemas conhecidos](/graph/known-issues#users).</span><span class="sxs-lookup"><span data-stu-id="0728d-125">For details, see the [known issues](/graph/known-issues#users) list.</span></span>

<span data-ttu-id="0728d-126">Para o usuário conectado:</span><span class="sxs-lookup"><span data-stu-id="0728d-126">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0728d-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0728d-127">Optional query parameters</span></span>

<span data-ttu-id="0728d-128">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0728d-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0728d-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0728d-129">Request headers</span></span>

| <span data-ttu-id="0728d-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0728d-130">Header</span></span>       | <span data-ttu-id="0728d-131">Valor</span><span class="sxs-lookup"><span data-stu-id="0728d-131">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="0728d-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="0728d-132">Authorization</span></span>  | <span data-ttu-id="0728d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0728d-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="0728d-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0728d-135">Content-Type</span></span>   | <span data-ttu-id="0728d-136">application/json</span><span class="sxs-lookup"><span data-stu-id="0728d-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0728d-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0728d-137">Request body</span></span>

<span data-ttu-id="0728d-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0728d-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0728d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0728d-139">Response</span></span>

<span data-ttu-id="0728d-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0728d-140">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="0728d-141">Esse método retorna `202 Accepted` quando a solicitação tenha sido processada com sucesso, mas o servidor requer mais tempo para concluir as operações de segundo plano relacionadas.</span><span class="sxs-lookup"><span data-stu-id="0728d-141">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="0728d-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0728d-142">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="0728d-143">Exemplo 1: Obter as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="0728d-143">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="0728d-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0728d-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0728d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0728d-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="0728d-146">C#</span><span class="sxs-lookup"><span data-stu-id="0728d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0728d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0728d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0728d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0728d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0728d-149">Java</span><span class="sxs-lookup"><span data-stu-id="0728d-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0728d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0728d-150">Response</span></span>
<span data-ttu-id="0728d-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0728d-151">Here is an example of the response.</span></span> <span data-ttu-id="0728d-152">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0728d-152">Note: The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "jobTitle": "Retail Manager",
   "mail": "AdeleV@contoso.onmicrosoft.com",
   "mobilePhone": "+1 425 555 0109",
   "officeLocation": "18/2111",
   "preferredLanguage": "en-US",
   "surname": "Vance",
   "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
   "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="0728d-153">Exemplo 2: Obter as propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="0728d-153">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="0728d-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0728d-154">Request</span></span>

<span data-ttu-id="0728d-155">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0728d-155">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0728d-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="0728d-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="0728d-157">C#</span><span class="sxs-lookup"><span data-stu-id="0728d-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0728d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0728d-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0728d-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0728d-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0728d-160">Java</span><span class="sxs-lookup"><span data-stu-id="0728d-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0728d-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="0728d-161">Response</span></span>

<span data-ttu-id="0728d-162">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="0728d-162">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
      "displayName": "Adele Vance",
      "givenName": "Adele",
      "jobTitle": "Retail Manager",
      "mail": "AdeleV@contoso.onmicrosoft.com",
      "mobilePhone": "+1 425 555 0109",
      "officeLocation": "18/2111",
      "preferredLanguage": "en-US",
      "surname": "Vance",
      "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
      "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```

## <a name="see-also"></a><span data-ttu-id="0728d-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="0728d-163">See also</span></span>

- [<span data-ttu-id="0728d-164">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="0728d-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0728d-165">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="0728d-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="0728d-166">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="0728d-166">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
