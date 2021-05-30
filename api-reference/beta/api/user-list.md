---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2636830f993626cc2d220c5a09543640f8da181f
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703542"
---
# <a name="list-users"></a><span data-ttu-id="cfc3a-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="cfc3a-103">List users</span></span>

<span data-ttu-id="cfc3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfc3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfc3a-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="cfc3a-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="cfc3a-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="cfc3a-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="cfc3a-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="cfc3a-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](user-get.md) para o usuário e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfc3a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfc3a-109">Permissions</span></span>

<span data-ttu-id="cfc3a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfc3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfc3a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfc3a-112">Permission type</span></span>      | <span data-ttu-id="cfc3a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfc3a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfc3a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfc3a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cfc3a-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cfc3a-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cfc3a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfc3a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfc3a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-117">Not supported.</span></span>    |
|<span data-ttu-id="cfc3a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfc3a-118">Application</span></span> | <span data-ttu-id="cfc3a-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfc3a-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfc3a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc3a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfc3a-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cfc3a-121">Optional query parameters</span></span>

<span data-ttu-id="cfc3a-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="cfc3a-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="cfc3a-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="cfc3a-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="cfc3a-126">Os parâmetros `$count` e `$search` não estão disponíveis no momento em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-126">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="cfc3a-p104">Certas propriedades não podem ser retornadas em uma coleção de usuário. As seguintes propriedades terão suporte apenas [ao recuperar um único usuário:](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving a single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

<span data-ttu-id="cfc3a-129">As propriedades a seguir não têm suporte em contas pessoais da Microsoft e serão `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-129">The following properties are not supported in personal Microsoft accounts and will be `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfc3a-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-130">Request headers</span></span>

| <span data-ttu-id="cfc3a-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfc3a-131">Header</span></span> | <span data-ttu-id="cfc3a-132">Valor</span><span class="sxs-lookup"><span data-stu-id="cfc3a-132">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="cfc3a-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfc3a-133">Authorization</span></span> | <span data-ttu-id="cfc3a-134">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="cfc3a-134">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="cfc3a-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="cfc3a-135">ConsistencyLevel</span></span> | <span data-ttu-id="cfc3a-136">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-136">eventual.</span></span> <span data-ttu-id="cfc3a-137">Este cabeçalho e `$count` são necessários ao usar `$search`, ou ao usar o `$filter` com o parâmetro de consulta `$orderby` ou `$filter` com o operador lógico `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-137">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter, or `$filter` with the `endsWith` logical operator.</span></span> <span data-ttu-id="cfc3a-138">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-138">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfc3a-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-139">Request body</span></span>

<span data-ttu-id="cfc3a-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfc3a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-141">Response</span></span>

<span data-ttu-id="cfc3a-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-142">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfc3a-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cfc3a-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="cfc3a-144">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="cfc3a-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-145">Request</span></span>

<span data-ttu-id="cfc3a-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfc3a-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc3a-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="cfc3a-148">C#</span><span class="sxs-lookup"><span data-stu-id="cfc3a-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfc3a-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfc3a-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfc3a-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfc3a-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfc3a-151">Java</span><span class="sxs-lookup"><span data-stu-id="cfc3a-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cfc3a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-152">Response</span></span>

<span data-ttu-id="cfc3a-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-153">The following is an example of the response.</span></span> 
><span data-ttu-id="cfc3a-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="cfc3a-155">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="cfc3a-155">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="cfc3a-156">Encontrar uma conta de usuário usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="cfc3a-156">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="cfc3a-157">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-157">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="cfc3a-158">O valor de **issuerAssignedId** deve ser o endereço de email da conta do usuário, não o nome de usuário principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="cfc3a-158">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="cfc3a-159">Se um UPN for usado, a resposta será uma lista em branco.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-159">If a UPN is used, the response will be an empty list.</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-160">Request</span></span>

<span data-ttu-id="cfc3a-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfc3a-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc3a-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="cfc3a-163">C#</span><span class="sxs-lookup"><span data-stu-id="cfc3a-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfc3a-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfc3a-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfc3a-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfc3a-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfc3a-166">Java</span><span class="sxs-lookup"><span data-stu-id="cfc3a-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cfc3a-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-167">Response</span></span>

<span data-ttu-id="cfc3a-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-168">The following is an example of the response.</span></span> 
> <span data-ttu-id="cfc3a-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="cfc3a-170">Exemplo 3: Obter usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="cfc3a-170">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-171">Request</span></span>

<span data-ttu-id="cfc3a-p107">A seguir está um exemplo de solicitação. Os detalhes da propriedade **signInActivity** requerem uma licença do Azure AD Premium P1/P2 e a permissão AuditLog.Read.All.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-p107">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>


# <a name="http"></a>[<span data-ttu-id="cfc3a-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc3a-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="cfc3a-175">C#</span><span class="sxs-lookup"><span data-stu-id="cfc3a-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfc3a-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfc3a-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfc3a-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfc3a-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfc3a-178">Java</span><span class="sxs-lookup"><span data-stu-id="cfc3a-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cfc3a-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-179">Response</span></span>

<span data-ttu-id="cfc3a-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-180">The following is an example of the response.</span></span> 
> <span data-ttu-id="cfc3a-181">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-181">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="cfc3a-182">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="cfc3a-182">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-183">Request</span></span>

<span data-ttu-id="cfc3a-p108">A seguir está um exemplo de solicitação. Os detalhes da propriedade **signInActivity** requerem uma licença do Azure AD Premium P1/P2 e a permissão AuditLog.Read.All.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-p108">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfc3a-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc3a-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="cfc3a-187">C#</span><span class="sxs-lookup"><span data-stu-id="cfc3a-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfc3a-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfc3a-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfc3a-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfc3a-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfc3a-190">Java</span><span class="sxs-lookup"><span data-stu-id="cfc3a-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cfc3a-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-191">Response</span></span>

<span data-ttu-id="cfc3a-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-192">The following is an example of the response.</span></span> 
> <span data-ttu-id="cfc3a-193">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-193">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="cfc3a-194">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="cfc3a-194">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-195">Request</span></span>

<span data-ttu-id="cfc3a-p109">A seguir está um exemplo de solicitação. Os detalhes da propriedade **signInActivity** requerem uma licença do Azure AD Premium P1/P2 e a permissão AuditLog.Read.All.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-p109">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_signin_last_time_range"
}-->
```http
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="cfc3a-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-198">Response</span></span>

<span data-ttu-id="cfc3a-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-199">The following is an example of the response.</span></span> 
> <span data-ttu-id="cfc3a-200">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-200">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="cfc3a-201">Exemplo 6: Obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="cfc3a-201">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-202">Request</span></span>

<span data-ttu-id="cfc3a-203">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-203">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cfc3a-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-204">Response</span></span>

<span data-ttu-id="cfc3a-205">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-205">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="cfc3a-206">Exemplo 7: Utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="cfc3a-206">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-207">Request</span></span>

<span data-ttu-id="cfc3a-208">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-208">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cfc3a-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-209">Response</span></span>

<span data-ttu-id="cfc3a-210">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-210">The following is an example of the response.</span></span>
><span data-ttu-id="cfc3a-211">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-211">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-8-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="cfc3a-212">Exemplo 8: utilize $filter para obter todos os usuários com um email que termina com “a@contoso.com”, incluindo uma contagem de objetos retornados, com os resultados pedidos por userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cfc3a-212">Example 8: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-213">Request</span></span>

<span data-ttu-id="cfc3a-214">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-214">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cfc3a-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc3a-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="cfc3a-216">C#</span><span class="sxs-lookup"><span data-stu-id="cfc3a-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfc3a-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfc3a-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfc3a-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfc3a-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfc3a-219">Java</span><span class="sxs-lookup"><span data-stu-id="cfc3a-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cfc3a-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-220">Response</span></span>

<span data-ttu-id="cfc3a-221">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-221">The following is an example of the response.</span></span>

><span data-ttu-id="cfc3a-222">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-222">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count": 1,
  "value": [
    {
      "displayName": "Grady Archie",
      "givenName": "Grady",
      "jobTitle": "Designer",
      "mail": "GradyA@contoso.com",
      "userPrincipalName": "GradyA@contoso.com",
      "id": "e8b753b5-4117-464e-9a08-713e1ff266b3"
      }
    ]
}
```

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="cfc3a-223">Exemplo 9: utilize $search para obter usuários com nomes de exibição que contenham as letras “wa”, incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="cfc3a-223">Example 9: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-224">Request</span></span>

<span data-ttu-id="cfc3a-225">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-225">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cfc3a-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-226">Response</span></span>

<span data-ttu-id="cfc3a-227">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-227">The following is an example of the response.</span></span>
><span data-ttu-id="cfc3a-228">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-228">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-10-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="cfc3a-229">Exemplo 10: utilize $search para obter grupos com nomes de exibição que contenham as letras “wa”, ou as letras para incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="cfc3a-229">Example 10: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-230">Request</span></span>

<span data-ttu-id="cfc3a-231">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-231">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cfc3a-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-232">Response</span></span>

<span data-ttu-id="cfc3a-233">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-233">The following is an example of the response.</span></span> 
> <span data-ttu-id="cfc3a-234">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-234">**Note:** The response object shown here might be shortened for readability.</span></span>

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


### <a name="example-11-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="cfc3a-235">Exemplo 11: use $filter para obter usuários que receberam uma licença específica</span><span class="sxs-lookup"><span data-stu-id="cfc3a-235">Example 11: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="cfc3a-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc3a-236">Request</span></span>

<span data-ttu-id="cfc3a-237">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-237">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="cfc3a-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc3a-238">Response</span></span>

<span data-ttu-id="cfc3a-239">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc3a-239">The following is an example of the response.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(id,mail,assignedLicenses)",
  "value": [
    {
      "id": "cb4954e8-467f-4a6d-a8c8-28b9034fadbc",
      "mail": "admin@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
    },
    {
      "id": "81a133c2-bdf2-4e67-8755-7264366b04ee",
      "mail": "DebraB@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
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
