---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2459c8a01facff8e233eb19482def8e18bec6957
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796854"
---
# <a name="list-users"></a><span data-ttu-id="c274d-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="c274d-103">List users</span></span>

<span data-ttu-id="c274d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c274d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c274d-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c274d-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c274d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c274d-106">Permissions</span></span>

<span data-ttu-id="c274d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c274d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c274d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c274d-109">Permission type</span></span>      | <span data-ttu-id="c274d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c274d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c274d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c274d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c274d-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c274d-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c274d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c274d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c274d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c274d-114">Not supported.</span></span>    |
|<span data-ttu-id="c274d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c274d-115">Application</span></span> | <span data-ttu-id="c274d-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c274d-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c274d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c274d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c274d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c274d-118">Optional query parameters</span></span>

<span data-ttu-id="c274d-119">Este método suporta os parâmetros de consulta [OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, `$filter`, e `$select`.</span><span class="sxs-lookup"><span data-stu-id="c274d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="c274d-120">Você pode usar `$search`na propriedade **displayName** .</span><span class="sxs-lookup"><span data-stu-id="c274d-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="c274d-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="c274d-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="c274d-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="c274d-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="c274d-123">Por padrão, apenas um conjunto limitado de propriedades é retornado ( **businessPhones** , **displayName** , **givenName** , **id** , **jobTitle** , **mail** , **mobilePhone** , **officeLocation** , **preferredLanguage** , **surname** e **userPrincipalName** ).</span><span class="sxs-lookup"><span data-stu-id="c274d-123">By default, only a limited set of properties are returned ( **businessPhones** , **displayName** , **givenName** , **id** , **jobTitle** , **mail** , **mobilePhone** , **officeLocation** , **preferredLanguage** , **surname** , and **userPrincipalName** ).</span></span> 

<span data-ttu-id="c274d-124">Para retornar um conjunto de propriedades alternativas, especifique o conjunto desejado de propriedades do [usuário](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="c274d-124">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="c274d-125">Por exemplo, para retornar **displayName** , **givenName** e **postalCode** , adicione o seguinte à sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="c274d-125">For example, to return **displayName** , **givenName** , and **postalCode** , add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="c274d-126">Determinadas propriedades não podem ser retornadas dentro de uma coleção de usuário.</span><span class="sxs-lookup"><span data-stu-id="c274d-126">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="c274d-127">As seguintes propriedades só possuem suporte ao [recuperar um único usuário](./user-get.md): **aboutMe** , **birthday** , **hireDate** , **interests** , **mySite** , **pastProjects** , **preferredName** , **responsibilities** , **schools** , **skills** , **mailboxSettings** .</span><span class="sxs-lookup"><span data-stu-id="c274d-127">The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe** , **birthday** , **hireDate** , **interests** , **mySite** , **pastProjects** , **preferredName** , **responsibilities** , **schools** , **skills** , **mailboxSettings** .</span></span>

## <a name="request-headers"></a><span data-ttu-id="c274d-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-128">Request headers</span></span>

| <span data-ttu-id="c274d-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c274d-129">Header</span></span>        | <span data-ttu-id="c274d-130">Valor</span><span class="sxs-lookup"><span data-stu-id="c274d-130">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="c274d-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c274d-131">Authorization</span></span> | <span data-ttu-id="c274d-132">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="c274d-132">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="c274d-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c274d-133">ConsistencyLevel</span></span> | <span data-ttu-id="c274d-134">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="c274d-134">eventual.</span></span> <span data-ttu-id="c274d-135">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="c274d-135">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="c274d-136">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="c274d-136">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c274d-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-137">Request body</span></span>

<span data-ttu-id="c274d-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c274d-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c274d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-139">Response</span></span>

<span data-ttu-id="c274d-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-140">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="c274d-141">Se uma coleção grande de usuários for retornada, você poderá usar a [paginação no seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="c274d-141">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="c274d-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c274d-142">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="c274d-143">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="c274d-143">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="c274d-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-144">Request</span></span>

<span data-ttu-id="c274d-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c274d-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```

#### <a name="response"></a><span data-ttu-id="c274d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-146">Response</span></span>

<span data-ttu-id="c274d-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-147">The following is an example of the response.</span></span>

><span data-ttu-id="c274d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c274d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="c274d-150">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="c274d-150">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="c274d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-151">Request</span></span>

<span data-ttu-id="c274d-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c274d-152">The following is an example of the request.</span></span>

><span data-ttu-id="c274d-153">**Observação:** Ao filtrar em **identidades** , você deve fornecer tanto **emissor** como **emissorAssignedId** .</span><span class="sxs-lookup"><span data-stu-id="c274d-153">**Note:** When filtering on **identities** , you must supply both **issuer** and **issuerAssignedId** .</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```

#### <a name="response"></a><span data-ttu-id="c274d-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-154">Response</span></span>

<span data-ttu-id="c274d-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-155">The following is an example of the response.</span></span> 

> <span data-ttu-id="c274d-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c274d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="c274d-158">Exemplo 3: Obter usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="c274d-158">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="c274d-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-159">Request</span></span>

<span data-ttu-id="c274d-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c274d-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,userPrincipalName,signInActivity
```

#### <a name="response"></a><span data-ttu-id="c274d-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-161">Response</span></span>

<span data-ttu-id="c274d-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-162">The following is an example of the response.</span></span>

><span data-ttu-id="c274d-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c274d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(displayName,userPrincipalName,signInActivity)",
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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="c274d-165">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="c274d-165">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="c274d-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-166">Request</span></span>

<span data-ttu-id="c274d-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c274d-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```

#### <a name="response"></a><span data-ttu-id="c274d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-168">Response</span></span>

<span data-ttu-id="c274d-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-169">The following is an example of the response.</span></span> 

> <span data-ttu-id="c274d-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c274d-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="c274d-172">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="c274d-172">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="c274d-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-173">Request</span></span>

<span data-ttu-id="c274d-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c274d-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="c274d-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-175">Response</span></span>

<span data-ttu-id="c274d-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-176">The following is an example of the response.</span></span> 

> <span data-ttu-id="c274d-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c274d-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="c274d-179">Exemplo 6: Obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="c274d-179">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="c274d-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-180">Request</span></span>

<span data-ttu-id="c274d-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c274d-181">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c274d-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-182">Response</span></span>

<span data-ttu-id="c274d-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-183">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="c274d-184">Exemplo 7: Utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="c274d-184">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c274d-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-185">Request</span></span>

<span data-ttu-id="c274d-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c274d-186">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c274d-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-187">Response</span></span>

<span data-ttu-id="c274d-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-188">The following is an example of the response.</span></span>

><span data-ttu-id="c274d-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c274d-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="c274d-191">Exemplo 8: Utilize $search para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="c274d-191">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c274d-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-192">Request</span></span>

<span data-ttu-id="c274d-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c274d-193">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c274d-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-194">Response</span></span>

<span data-ttu-id="c274d-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-195">The following is an example of the response.</span></span>

><span data-ttu-id="c274d-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c274d-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="c274d-198">Exemplo 9: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'wa', ou as letras para incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="c274d-198">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c274d-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c274d-199">Request</span></span>

<span data-ttu-id="c274d-200">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c274d-200">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c274d-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="c274d-201">Response</span></span>

<span data-ttu-id="c274d-202">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c274d-202">The following is an example of the response.</span></span>

> <span data-ttu-id="c274d-p114">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c274d-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
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
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
