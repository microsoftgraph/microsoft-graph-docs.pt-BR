---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para acessar o nível superior '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1c3151174276ad4bcb9fdfb89550609aebaba1e5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415292"
---
# <a name="list-childfolders"></a><span data-ttu-id="9d5ef-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="9d5ef-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d5ef-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/mailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d5ef-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d5ef-107">Permissions</span></span>

<span data-ttu-id="9d5ef-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d5ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d5ef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d5ef-110">Permission type</span></span>                        | <span data-ttu-id="9d5ef-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d5ef-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="9d5ef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d5ef-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d5ef-113">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d5ef-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="9d5ef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d5ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d5ef-115">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d5ef-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="9d5ef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d5ef-116">Application</span></span>                            | <span data-ttu-id="9d5ef-117">Mail. ReadBasic. All, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d5ef-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="9d5ef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d5ef-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d5ef-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9d5ef-119">Optional query parameters</span></span>

<span data-ttu-id="9d5ef-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d5ef-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d5ef-121">Request headers</span></span>

| <span data-ttu-id="9d5ef-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9d5ef-122">Name</span></span>          | <span data-ttu-id="9d5ef-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d5ef-123">Type</span></span>   | <span data-ttu-id="9d5ef-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d5ef-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="9d5ef-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d5ef-125">Authorization</span></span> | <span data-ttu-id="9d5ef-126">string</span><span class="sxs-lookup"><span data-stu-id="9d5ef-126">string</span></span> | <span data-ttu-id="9d5ef-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d5ef-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d5ef-129">Request body</span></span>

<span data-ttu-id="9d5ef-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d5ef-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d5ef-131">Response</span></span>

<span data-ttu-id="9d5ef-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d5ef-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9d5ef-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="9d5ef-134">Exemplo 1: listar pastas de email</span><span class="sxs-lookup"><span data-stu-id="9d5ef-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="9d5ef-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d5ef-135">Request</span></span>

<span data-ttu-id="9d5ef-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-136">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9d5ef-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d5ef-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9d5ef-138">C#</span><span class="sxs-lookup"><span data-stu-id="9d5ef-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d5ef-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d5ef-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d5ef-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9d5ef-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="9d5ef-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d5ef-141">Response</span></span>

<span data-ttu-id="9d5ef-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-142">The following is an example of the response.</span></span>

> <span data-ttu-id="9d5ef-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9d5ef-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-144">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="9d5ef-145">Exemplo 2: listar pastas de pesquisa de email</span><span class="sxs-lookup"><span data-stu-id="9d5ef-145">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="9d5ef-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d5ef-146">Request</span></span>

<span data-ttu-id="9d5ef-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-147">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9d5ef-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d5ef-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9d5ef-149">C#</span><span class="sxs-lookup"><span data-stu-id="9d5ef-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d5ef-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d5ef-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d5ef-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9d5ef-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9d5ef-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d5ef-152">Response</span></span>

<span data-ttu-id="9d5ef-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-153">The following is an example of the response.</span></span>

> <span data-ttu-id="9d5ef-154">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-154">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9d5ef-155">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d5ef-155">All the properties will be returned from an actual call.</span></span>

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
