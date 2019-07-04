---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a49e86b8aaccbf87e8c80f69659b648b3186405
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456782"
---
# <a name="list-users"></a><span data-ttu-id="ee292-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="ee292-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee292-104">Recuperar uma lista de objetos user.</span><span class="sxs-lookup"><span data-stu-id="ee292-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee292-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee292-105">Permissions</span></span>

<span data-ttu-id="ee292-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee292-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee292-108">Permission type</span></span>      | <span data-ttu-id="ee292-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee292-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee292-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee292-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee292-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee292-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee292-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee292-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee292-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee292-113">Not supported.</span></span>    |
|<span data-ttu-id="ee292-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee292-114">Application</span></span> | <span data-ttu-id="ee292-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee292-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee292-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee292-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee292-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee292-117">Optional query parameters</span></span>

<span data-ttu-id="ee292-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee292-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee292-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee292-119">Request headers</span></span>
| <span data-ttu-id="ee292-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee292-120">Header</span></span>        | <span data-ttu-id="ee292-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ee292-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="ee292-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee292-122">Authorization</span></span> | <span data-ttu-id="ee292-123">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="ee292-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="ee292-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee292-124">Content-Type</span></span>  | <span data-ttu-id="ee292-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee292-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="ee292-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee292-126">Request body</span></span>

<span data-ttu-id="ee292-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee292-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee292-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee292-128">Response</span></span>

<span data-ttu-id="ee292-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee292-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee292-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee292-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee292-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee292-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ee292-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee292-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ee292-133">C#</span><span class="sxs-lookup"><span data-stu-id="ee292-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee292-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ee292-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ee292-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee292-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee292-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee292-136">Response</span></span>

<span data-ttu-id="ee292-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee292-137">Here is an example of the response.</span></span> <span data-ttu-id="ee292-138">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="ee292-138">Note: The response object shown here may be truncated for brevity.</span></span> 

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
