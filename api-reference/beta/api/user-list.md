---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13550b7a76c7cd9cab1ba43ce5672fcfcf5afe14
ms.sourcegitcommit: 8ef30790a4d7aa94879df93773eae80b37abbfa4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37203953"
---
# <a name="list-users"></a><span data-ttu-id="c2962-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="c2962-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2962-104">Recuperar uma lista de objetos user.</span><span class="sxs-lookup"><span data-stu-id="c2962-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2962-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2962-105">Permissions</span></span>

<span data-ttu-id="c2962-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2962-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2962-108">Permission type</span></span>      | <span data-ttu-id="c2962-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2962-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2962-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2962-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2962-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c2962-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c2962-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2962-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2962-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2962-113">Not supported.</span></span>    |
|<span data-ttu-id="c2962-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2962-114">Application</span></span> | <span data-ttu-id="c2962-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2962-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2962-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2962-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2962-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2962-117">Optional query parameters</span></span>

<span data-ttu-id="c2962-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c2962-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2962-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2962-119">Request headers</span></span>
| <span data-ttu-id="c2962-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2962-120">Header</span></span>        | <span data-ttu-id="c2962-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c2962-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="c2962-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2962-122">Authorization</span></span> | <span data-ttu-id="c2962-123">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="c2962-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="c2962-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2962-124">Content-Type</span></span>  | <span data-ttu-id="c2962-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2962-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="c2962-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2962-126">Request body</span></span>

<span data-ttu-id="c2962-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2962-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2962-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2962-128">Response</span></span>

<span data-ttu-id="c2962-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2962-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2962-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2962-130">Example</span></span>

### <a name="example-1-list-all-users"></a><span data-ttu-id="c2962-131">Exemplo 1: listar todos os usuários</span><span class="sxs-lookup"><span data-stu-id="c2962-131">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="c2962-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2962-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2962-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2962-133">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2962-134">C#</span><span class="sxs-lookup"><span data-stu-id="c2962-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2962-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2962-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2962-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2962-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c2962-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2962-137">Response</span></span>

<span data-ttu-id="c2962-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2962-138">Here is an example of the response.</span></span> 

><span data-ttu-id="c2962-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c2962-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c2962-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2962-140">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="c2962-141">Exemplo 2: localizar uma conta de usuário usando o nome de entrada</span><span class="sxs-lookup"><span data-stu-id="c2962-141">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="c2962-142">Encontrar uma conta de usuário em um locatário B2C usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="c2962-142">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="c2962-143">Essa solicitação pode ser usada por um suporte técnico para encontrar uma conta de usuário do cliente, em um locatário B2C (neste exemplo, o locatário B2C é contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="c2962-143">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="c2962-144">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="c2962-144">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="c2962-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2962-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```http
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```

#### <a name="response"></a><span data-ttu-id="c2962-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2962-146">Response</span></span>

<span data-ttu-id="c2962-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2962-147">Here is an example of the response.</span></span> 

> <span data-ttu-id="c2962-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2962-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
