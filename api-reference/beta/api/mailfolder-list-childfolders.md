---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para acessar o nível superior '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 023ead7f1dfaf671be8c9d32a678a92eee348005
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880039"
---
# <a name="list-childfolders"></a><span data-ttu-id="7235c-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="7235c-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7235c-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/mailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="7235c-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="7235c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7235c-107">Permissions</span></span>

<span data-ttu-id="7235c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7235c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7235c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7235c-110">Permission type</span></span>                        | <span data-ttu-id="7235c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7235c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="7235c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7235c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7235c-113">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7235c-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="7235c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7235c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7235c-115">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7235c-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="7235c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7235c-116">Application</span></span>                            | <span data-ttu-id="7235c-117">Mail. ReadBasic. All, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7235c-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="7235c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7235c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7235c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7235c-119">Optional query parameters</span></span>

<span data-ttu-id="7235c-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7235c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7235c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7235c-121">Request headers</span></span>

| <span data-ttu-id="7235c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7235c-122">Name</span></span>          | <span data-ttu-id="7235c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7235c-123">Type</span></span>   | <span data-ttu-id="7235c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7235c-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="7235c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7235c-125">Authorization</span></span> | <span data-ttu-id="7235c-126">string</span><span class="sxs-lookup"><span data-stu-id="7235c-126">string</span></span> | <span data-ttu-id="7235c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7235c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7235c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7235c-129">Request body</span></span>

<span data-ttu-id="7235c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7235c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7235c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7235c-131">Response</span></span>

<span data-ttu-id="7235c-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7235c-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7235c-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7235c-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="7235c-134">Exemplo 1: listar pastas de email</span><span class="sxs-lookup"><span data-stu-id="7235c-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="7235c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7235c-135">Request</span></span>

<span data-ttu-id="7235c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7235c-136">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7235c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7235c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7235c-138">C#</span><span class="sxs-lookup"><span data-stu-id="7235c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7235c-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="7235c-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7235c-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7235c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7235c-141">Java</span><span class="sxs-lookup"><span data-stu-id="7235c-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="7235c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7235c-142">Response</span></span>

<span data-ttu-id="7235c-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7235c-143">The following is an example of the response.</span></span>

> <span data-ttu-id="7235c-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7235c-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7235c-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7235c-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "AAMkAGVmMDEzA",
      "displayName": "Internal Screens",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 2,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Project Falcon",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders"
    }
  ]
}
```

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="7235c-146">Exemplo 2: listar pastas de pesquisa de email</span><span class="sxs-lookup"><span data-stu-id="7235c-146">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="7235c-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7235c-147">Request</span></span>

<span data-ttu-id="7235c-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7235c-148">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7235c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="7235c-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7235c-150">C#</span><span class="sxs-lookup"><span data-stu-id="7235c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7235c-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="7235c-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7235c-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7235c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7235c-153">Java</span><span class="sxs-lookup"><span data-stu-id="7235c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-childfolders-of-searchfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7235c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7235c-154">Response</span></span>

<span data-ttu-id="7235c-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7235c-155">The following is an example of the response.</span></span>

> <span data-ttu-id="7235c-156">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7235c-156">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7235c-157">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7235c-157">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMz",
      "displayName": "Get MyAnalytics",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 6,
      "totalItemCount": 6,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'MyAnalytics')"
    },
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMy",
      "displayName": "Action Required",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 4,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
