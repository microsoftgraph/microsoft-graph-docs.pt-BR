---
title: Obter usuário
description: Recupere o **usuário** do diretório simples que corresponde a esse **educationUser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0c7c67d6bf8e913b6cff1fb6a523e30bdb8e232f
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720270"
---
# <a name="get-user"></a><span data-ttu-id="1af5c-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="1af5c-103">Get user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1af5c-104">Recupere o **usuário** do diretório simples que corresponde a esse **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="1af5c-104">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="1af5c-105">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="1af5c-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="1af5c-106">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="1af5c-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="1af5c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1af5c-107">Permissions</span></span>
<span data-ttu-id="1af5c-108">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1af5c-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="1af5c-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1af5c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1af5c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1af5c-110">Permission type</span></span>      | <span data-ttu-id="1af5c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1af5c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1af5c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1af5c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="1af5c-113">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1af5c-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="1af5c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1af5c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1af5c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1af5c-115">Not supported.</span></span>  |
|<span data-ttu-id="1af5c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1af5c-116">Application</span></span> | <span data-ttu-id="1af5c-117">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1af5c-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="1af5c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1af5c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="1af5c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1af5c-119">Request headers</span></span>
| <span data-ttu-id="1af5c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1af5c-120">Header</span></span>       | <span data-ttu-id="1af5c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1af5c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1af5c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1af5c-122">Authorization</span></span>  | <span data-ttu-id="1af5c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1af5c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1af5c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1af5c-125">Request body</span></span>
<span data-ttu-id="1af5c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1af5c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1af5c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1af5c-127">Response</span></span>
<span data-ttu-id="1af5c-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1af5c-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1af5c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1af5c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1af5c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1af5c-130">Request</span></span>
<span data-ttu-id="1af5c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1af5c-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1af5c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1af5c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/user
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1af5c-133">C#</span><span class="sxs-lookup"><span data-stu-id="1af5c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1af5c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1af5c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1af5c-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1af5c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1af5c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1af5c-136">Response</span></span>
<span data-ttu-id="1af5c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1af5c-137">The following is an example of the response.</span></span> 

><span data-ttu-id="1af5c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1af5c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
