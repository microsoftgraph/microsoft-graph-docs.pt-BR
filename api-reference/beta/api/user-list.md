---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92ad556051ddddaa767384e46c92b894e152883c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937466"
---
# <a name="list-users"></a><span data-ttu-id="96710-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="96710-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96710-104">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="96710-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="96710-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="96710-105">Permissions</span></span>

<span data-ttu-id="96710-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96710-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96710-108">Permission type</span></span>      | <span data-ttu-id="96710-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96710-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96710-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96710-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96710-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96710-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="96710-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96710-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96710-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96710-113">Not supported.</span></span>    |
|<span data-ttu-id="96710-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96710-114">Application</span></span> | <span data-ttu-id="96710-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96710-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96710-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96710-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96710-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="96710-117">Optional query parameters</span></span>

<span data-ttu-id="96710-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="96710-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96710-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96710-119">Request headers</span></span>
| <span data-ttu-id="96710-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96710-120">Header</span></span>        | <span data-ttu-id="96710-121">Valor</span><span class="sxs-lookup"><span data-stu-id="96710-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="96710-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="96710-122">Authorization</span></span> | <span data-ttu-id="96710-123">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="96710-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="96710-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96710-124">Content-Type</span></span>  | <span data-ttu-id="96710-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96710-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="96710-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96710-126">Request body</span></span>

<span data-ttu-id="96710-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96710-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96710-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="96710-128">Response</span></span>

<span data-ttu-id="96710-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96710-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96710-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96710-130">Example</span></span>

### <a name="example-1-list-all-users"></a><span data-ttu-id="96710-131">Exemplo 1: listar todos os usuários</span><span class="sxs-lookup"><span data-stu-id="96710-131">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="96710-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96710-132">Request</span></span>

<span data-ttu-id="96710-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96710-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96710-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="96710-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96710-135">C#</span><span class="sxs-lookup"><span data-stu-id="96710-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96710-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96710-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96710-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96710-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96710-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="96710-138">Response</span></span>

<span data-ttu-id="96710-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96710-139">The following is an example of the response.</span></span> 
><span data-ttu-id="96710-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96710-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="96710-142">Exemplo 2: localizar uma conta de usuário usando o nome de entrada</span><span class="sxs-lookup"><span data-stu-id="96710-142">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="96710-143">Encontrar uma conta de usuário em um locatário B2C usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="96710-143">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="96710-144">Essa solicitação pode ser usada por um suporte técnico para encontrar uma conta de usuário do cliente, em um locatário B2C (neste exemplo, o locatário B2C é contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="96710-144">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="96710-145">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="96710-145">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="96710-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96710-146">Request</span></span>

<span data-ttu-id="96710-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96710-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96710-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="96710-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96710-149">C#</span><span class="sxs-lookup"><span data-stu-id="96710-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96710-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96710-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96710-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96710-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96710-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="96710-152">Response</span></span>

<span data-ttu-id="96710-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96710-153">The following is an example of the response.</span></span> 
> <span data-ttu-id="96710-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96710-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3--list-users-including-their-last-sign-in-time"></a><span data-ttu-id="96710-156">Exemplo 3: listar usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="96710-156">Example 3:  List users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="96710-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96710-157">Request</span></span>

<span data-ttu-id="96710-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96710-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName, signInActivity
```

#### <a name="response"></a><span data-ttu-id="96710-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="96710-159">Response</span></span>

<span data-ttu-id="96710-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96710-160">The following is an example of the response.</span></span> 
> <span data-ttu-id="96710-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96710-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
