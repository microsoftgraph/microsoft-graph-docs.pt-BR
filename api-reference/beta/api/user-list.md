---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ab92e0634638ffd37d6c6f38327bdc6385193032
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400848"
---
# <a name="list-users"></a><span data-ttu-id="2f977-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="2f977-103">List users</span></span>

<span data-ttu-id="2f977-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f977-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f977-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="2f977-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="2f977-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="2f977-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="2f977-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="2f977-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="2f977-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](user-get.md) para o usuário e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="2f977-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f977-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f977-109">Permissions</span></span>

<span data-ttu-id="2f977-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f977-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f977-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f977-112">Permission type</span></span>      | <span data-ttu-id="2f977-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f977-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f977-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f977-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2f977-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2f977-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2f977-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f977-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f977-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f977-117">Not supported.</span></span>    |
|<span data-ttu-id="2f977-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f977-118">Application</span></span> | <span data-ttu-id="2f977-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f977-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f977-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f977-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f977-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f977-121">Optional query parameters</span></span>

<span data-ttu-id="2f977-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="2f977-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="2f977-123">Você pode usar `$search`na propriedade**displayName**.</span><span class="sxs-lookup"><span data-stu-id="2f977-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="2f977-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="2f977-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="2f977-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="2f977-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f977-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-126">Request headers</span></span>

| <span data-ttu-id="2f977-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f977-127">Header</span></span> | <span data-ttu-id="2f977-128">Valor</span><span class="sxs-lookup"><span data-stu-id="2f977-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="2f977-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f977-129">Authorization</span></span> | <span data-ttu-id="2f977-130">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="2f977-130">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="2f977-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="2f977-131">ConsistencyLevel</span></span> | <span data-ttu-id="2f977-132">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="2f977-132">eventual.</span></span> <span data-ttu-id="2f977-133">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="2f977-133">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="2f977-134">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="2f977-134">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f977-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-135">Request body</span></span>

<span data-ttu-id="2f977-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f977-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f977-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-137">Response</span></span>

<span data-ttu-id="2f977-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-138">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f977-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2f977-139">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="2f977-140">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="2f977-140">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="2f977-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-141">Request</span></span>

<span data-ttu-id="2f977-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f977-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f977-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f977-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="2f977-144">C#</span><span class="sxs-lookup"><span data-stu-id="2f977-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f977-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f977-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f977-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f977-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2f977-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-147">Response</span></span>

<span data-ttu-id="2f977-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-148">The following is an example of the response.</span></span> 
><span data-ttu-id="2f977-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f977-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value":[
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "otherMails":["contoso1@gmail.com"],
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="2f977-151">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="2f977-151">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="2f977-152">Encontrar uma conta de usuário usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="2f977-152">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="2f977-153">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="2f977-153">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="2f977-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-154">Request</span></span>

<span data-ttu-id="2f977-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f977-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f977-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f977-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="2f977-157">C#</span><span class="sxs-lookup"><span data-stu-id="2f977-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f977-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f977-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f977-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f977-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2f977-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-160">Response</span></span>

<span data-ttu-id="2f977-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-161">The following is an example of the response.</span></span> 
> <span data-ttu-id="2f977-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f977-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "displayName": "John Smith"
    }
  ]
}
```

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="2f977-164">Exemplo 3: Obter usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="2f977-164">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="2f977-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-165">Request</span></span>

<span data-ttu-id="2f977-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f977-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f977-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f977-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="2f977-168">C#</span><span class="sxs-lookup"><span data-stu-id="2f977-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f977-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f977-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f977-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f977-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2f977-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-171">Response</span></span>

<span data-ttu-id="2f977-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-172">The following is an example of the response.</span></span> 
> <span data-ttu-id="2f977-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f977-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="2f977-175">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="2f977-175">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="2f977-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-176">Request</span></span>

<span data-ttu-id="2f977-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f977-177">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="2f977-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f977-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="2f977-179">C#</span><span class="sxs-lookup"><span data-stu-id="2f977-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f977-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f977-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f977-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f977-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f977-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-182">Response</span></span>

<span data-ttu-id="2f977-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-183">The following is an example of the response.</span></span> 
> <span data-ttu-id="2f977-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f977-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
  "value": [
    {
      "displayName": "Eric Solomon",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    }
  ]
}
```

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="2f977-186">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="2f977-186">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="2f977-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-187">Request</span></span>

<span data-ttu-id="2f977-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f977-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="2f977-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f977-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="2f977-190">C#</span><span class="sxs-lookup"><span data-stu-id="2f977-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f977-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f977-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f977-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f977-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f977-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-193">Response</span></span>

<span data-ttu-id="2f977-194">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-194">The following is an example of the response.</span></span> 
> <span data-ttu-id="2f977-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f977-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-05-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-04-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="2f977-197">Exemplo 6: Obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="2f977-197">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="2f977-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-198">Request</span></span>

<span data-ttu-id="2f977-199">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f977-199">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f977-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f977-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2f977-201">C#</span><span class="sxs-lookup"><span data-stu-id="2f977-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f977-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f977-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f977-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f977-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f977-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-204">Response</span></span>

<span data-ttu-id="2f977-205">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-205">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="2f977-206">893</span><span class="sxs-lookup"><span data-stu-id="2f977-206">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="2f977-207">Exemplo 7: Utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="2f977-207">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2f977-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-208">Request</span></span>

<span data-ttu-id="2f977-209">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f977-209">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f977-210">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f977-210">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2f977-211">C#</span><span class="sxs-lookup"><span data-stu-id="2f977-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f977-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f977-212">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f977-213">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f977-213">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f977-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-214">Response</span></span>

<span data-ttu-id="2f977-215">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-215">The following is an example of the response.</span></span>
><span data-ttu-id="2f977-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f977-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mail":"a@contoso.com",
      "mailNickname":"a_contoso.com#EXT#",
      "otherMails":["a@contoso.com"],
      "proxyAddresses":["SMTP:a@contoso.com"],
      "userPrincipalName":"a_contoso.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="2f977-218">Exemplo 8: Utilize $search para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="2f977-218">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2f977-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-219">Request</span></span>

<span data-ttu-id="2f977-220">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f977-220">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f977-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f977-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2f977-222">C#</span><span class="sxs-lookup"><span data-stu-id="2f977-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-wa-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f977-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f977-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-wa-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f977-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f977-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-wa-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f977-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-225">Response</span></span>

<span data-ttu-id="2f977-226">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-226">The following is an example of the response.</span></span>
><span data-ttu-id="2f977-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f977-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    }
  ]
}

```

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="2f977-229">Exemplo 9: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'wa', ou as letras para incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="2f977-229">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2f977-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f977-230">Request</span></span>

<span data-ttu-id="2f977-231">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f977-231">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="2f977-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f977-232">Response</span></span>

<span data-ttu-id="2f977-233">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f977-233">The following is an example of the response.</span></span> 
> <span data-ttu-id="2f977-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f977-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    },
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
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