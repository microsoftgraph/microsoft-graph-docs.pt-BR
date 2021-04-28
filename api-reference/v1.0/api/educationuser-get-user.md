---
title: Obter usuário
description: Recupere o **usuário** do diretório simples que corresponde a esse **educationUser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1260845c6956618fc904ae9964f2dd7246fbf4b7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051428"
---
# <a name="get-user"></a><span data-ttu-id="7ea06-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="7ea06-103">Get user</span></span>

<span data-ttu-id="7ea06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ea06-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ea06-105">Recupere o **usuário** do diretório simples que corresponde a esse **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="7ea06-105">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="7ea06-106">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="7ea06-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="7ea06-107">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="7ea06-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ea06-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ea06-108">Permissions</span></span>
<span data-ttu-id="7ea06-109">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7ea06-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="7ea06-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ea06-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ea06-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ea06-111">Permission type</span></span>      | <span data-ttu-id="7ea06-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ea06-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ea06-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ea06-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="7ea06-114">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ea06-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="7ea06-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ea06-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7ea06-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ea06-116">Not supported.</span></span>  |
|<span data-ttu-id="7ea06-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ea06-117">Application</span></span> | <span data-ttu-id="7ea06-118">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ea06-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="7ea06-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ea06-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="7ea06-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ea06-120">Request headers</span></span>
| <span data-ttu-id="7ea06-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ea06-121">Header</span></span>       | <span data-ttu-id="7ea06-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7ea06-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ea06-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ea06-123">Authorization</span></span>  | <span data-ttu-id="7ea06-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ea06-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ea06-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ea06-126">Request body</span></span>
<span data-ttu-id="7ea06-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ea06-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7ea06-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ea06-128">Response</span></span>
<span data-ttu-id="7ea06-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ea06-129">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ea06-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ea06-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ea06-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ea06-131">Request</span></span>
<span data-ttu-id="7ea06-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ea06-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ea06-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ea06-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/user
```
# <a name="c"></a>[<span data-ttu-id="7ea06-134">C#</span><span class="sxs-lookup"><span data-stu-id="7ea06-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ea06-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ea06-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ea06-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ea06-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ea06-137">Java</span><span class="sxs-lookup"><span data-stu-id="7ea06-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7ea06-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ea06-138">Response</span></span>
<span data-ttu-id="7ea06-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ea06-139">The following is an example of the response.</span></span> 

><span data-ttu-id="7ea06-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7ea06-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

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
```

<!-- uuid: FC4AAF57-A0ED-4899-B104-A8B89B72AD5A
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

