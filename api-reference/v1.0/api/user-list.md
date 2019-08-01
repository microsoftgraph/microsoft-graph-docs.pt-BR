---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 362716388f5c479e4b8c4a0009403817fcc80515
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026786"
---
# <a name="list-users"></a><span data-ttu-id="812cd-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="812cd-103">List users</span></span>

<span data-ttu-id="812cd-104">Recuperar uma lista de objetos user.</span><span class="sxs-lookup"><span data-stu-id="812cd-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="812cd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="812cd-105">Permissions</span></span>

<span data-ttu-id="812cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="812cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="812cd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="812cd-108">Permission type</span></span>      | <span data-ttu-id="812cd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="812cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="812cd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="812cd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="812cd-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="812cd-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="812cd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="812cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="812cd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="812cd-113">Not supported.</span></span>    |
|<span data-ttu-id="812cd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="812cd-114">Application</span></span> | <span data-ttu-id="812cd-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="812cd-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="812cd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="812cd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="812cd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="812cd-117">Optional query parameters</span></span>

<span data-ttu-id="812cd-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="812cd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="812cd-119">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** e **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="812cd-119">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> 

<span data-ttu-id="812cd-120">Para retornar um conjunto de propriedades alternativas, especifique o conjunto desejado de propriedades do [usuário](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="812cd-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="812cd-121">Por exemplo, para retornar**displayName**, **givenName** e **postalCode**, adicione o seguinte à sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="812cd-121">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

<span data-ttu-id="812cd-122">Determinadas propriedades não podem ser retornadas dentro de uma coleção de usuário.</span><span class="sxs-lookup"><span data-stu-id="812cd-122">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="812cd-123">As seguintes propriedades só possuem suporte ao [recuperar um único usuário](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="812cd-123">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings**</span></span>

## <a name="request-headers"></a><span data-ttu-id="812cd-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="812cd-124">Request headers</span></span>

| <span data-ttu-id="812cd-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="812cd-125">Header</span></span>        | <span data-ttu-id="812cd-126">Valor</span><span class="sxs-lookup"><span data-stu-id="812cd-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="812cd-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="812cd-127">Authorization</span></span> | <span data-ttu-id="812cd-128">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="812cd-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="812cd-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="812cd-129">Content-Type</span></span>  | <span data-ttu-id="812cd-130">application/json</span><span class="sxs-lookup"><span data-stu-id="812cd-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="812cd-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="812cd-131">Request body</span></span>

<span data-ttu-id="812cd-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="812cd-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="812cd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="812cd-133">Response</span></span>

<span data-ttu-id="812cd-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="812cd-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="812cd-135">Se uma coleção grande de usuários for retornada, você poderá usar a [paginação no seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="812cd-135">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="812cd-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="812cd-136">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="812cd-137">Exemplo 1: Solicitação de usuários padrão</span><span class="sxs-lookup"><span data-stu-id="812cd-137">Example 1: Standard users request</span></span>

<span data-ttu-id="812cd-138">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="812cd-138">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> <span data-ttu-id="812cd-139">Este exemplo ilustra a solicitação padrão e a resposta.</span><span class="sxs-lookup"><span data-stu-id="812cd-139">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="812cd-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="812cd-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="812cd-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="812cd-141">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="812cd-142">C#</span><span class="sxs-lookup"><span data-stu-id="812cd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="812cd-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="812cd-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="812cd-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="812cd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="812cd-145">Java</span><span class="sxs-lookup"><span data-stu-id="812cd-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="812cd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="812cd-146">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="812cd-147">Exemplo 2: Solicitação de usuários usando $select</span><span class="sxs-lookup"><span data-stu-id="812cd-147">Example 2: Users request using $select</span></span>

<span data-ttu-id="812cd-148">Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="812cd-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="812cd-149">Por exemplo, para retornar **displayName**, **givenName** e **postalCode**, você incluiria o seguinte na sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="812cd-149">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="812cd-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="812cd-150">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="812cd-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="812cd-151">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="812cd-152">C#</span><span class="sxs-lookup"><span data-stu-id="812cd-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="812cd-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="812cd-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="812cd-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="812cd-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="812cd-155">Java</span><span class="sxs-lookup"><span data-stu-id="812cd-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-properties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="812cd-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="812cd-156">Response</span></span>

<span data-ttu-id="812cd-157">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="812cd-157">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
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
