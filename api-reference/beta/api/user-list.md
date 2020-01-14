---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b151a097f733064e250e3df631671bc1ec4fc5e
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023093"
---
# <a name="list-users"></a><span data-ttu-id="1c66a-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="1c66a-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c66a-104">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="1c66a-104">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="1c66a-105">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="1c66a-105">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="1c66a-106">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="1c66a-106">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="1c66a-107">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](user-get.md) para o usuário e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="1c66a-107">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the group and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c66a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c66a-108">Permissions</span></span>

<span data-ttu-id="1c66a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c66a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c66a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c66a-111">Permission type</span></span>      | <span data-ttu-id="1c66a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c66a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c66a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c66a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1c66a-114">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c66a-114">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1c66a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c66a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c66a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c66a-116">Not supported.</span></span>    |
|<span data-ttu-id="1c66a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c66a-117">Application</span></span> | <span data-ttu-id="1c66a-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c66a-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c66a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c66a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c66a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c66a-120">Optional query parameters</span></span>

<span data-ttu-id="1c66a-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c66a-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c66a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c66a-122">Request headers</span></span>
| <span data-ttu-id="1c66a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c66a-123">Header</span></span>        | <span data-ttu-id="1c66a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1c66a-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="1c66a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c66a-125">Authorization</span></span> | <span data-ttu-id="1c66a-126">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="1c66a-126">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="1c66a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c66a-127">Content-Type</span></span>  | <span data-ttu-id="1c66a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1c66a-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="1c66a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c66a-129">Request body</span></span>

<span data-ttu-id="1c66a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c66a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c66a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c66a-131">Response</span></span>

<span data-ttu-id="1c66a-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c66a-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c66a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c66a-133">Example</span></span>

### <a name="example-1-list-all-users"></a><span data-ttu-id="1c66a-134">Exemplo 1: listar todos os usuários</span><span class="sxs-lookup"><span data-stu-id="1c66a-134">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="1c66a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c66a-135">Request</span></span>

<span data-ttu-id="1c66a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c66a-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1c66a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c66a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c66a-138">C#</span><span class="sxs-lookup"><span data-stu-id="1c66a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c66a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c66a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c66a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c66a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1c66a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c66a-141">Response</span></span>

<span data-ttu-id="1c66a-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c66a-142">The following is an example of the response.</span></span> 
><span data-ttu-id="1c66a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c66a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="1c66a-145">Exemplo 2: localizar uma conta de usuário usando o nome de entrada</span><span class="sxs-lookup"><span data-stu-id="1c66a-145">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="1c66a-146">Encontrar uma conta de usuário em um locatário B2C usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="1c66a-146">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="1c66a-147">Essa solicitação pode ser usada por um suporte técnico para encontrar uma conta de usuário do cliente, em um locatário B2C (neste exemplo, o locatário B2C é contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="1c66a-147">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="1c66a-148">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="1c66a-148">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="1c66a-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c66a-149">Request</span></span>

<span data-ttu-id="1c66a-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c66a-150">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1c66a-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c66a-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c66a-152">C#</span><span class="sxs-lookup"><span data-stu-id="1c66a-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c66a-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c66a-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c66a-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c66a-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c66a-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c66a-155">Response</span></span>

<span data-ttu-id="1c66a-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c66a-156">The following is an example of the response.</span></span> 
> <span data-ttu-id="1c66a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c66a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 108

{
  "value": [
    {
      "displayName": "John Smith",
      "id": "4c7be08b-361f-41a8-b1ef-1712f7a3dfb2"
    }
  ]
}
```

### <a name="example-3--list-users-including-their-last-sign-in-time"></a><span data-ttu-id="1c66a-159">Exemplo 3: listar usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="1c66a-159">Example 3:  List users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="1c66a-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c66a-160">Request</span></span>

<span data-ttu-id="1c66a-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c66a-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1c66a-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c66a-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName, signInActivity
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c66a-163">C#</span><span class="sxs-lookup"><span data-stu-id="1c66a-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c66a-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c66a-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c66a-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c66a-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c66a-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c66a-166">Response</span></span>

<span data-ttu-id="1c66a-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c66a-167">The following is an example of the response.</span></span> 
> <span data-ttu-id="1c66a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c66a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(displayName,userPrincipalName,signInActivity)",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-07-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
