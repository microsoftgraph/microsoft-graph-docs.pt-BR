---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para acessar o nível superior '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2d99b33d3d9ba90b1ad19b204eb93db133c09cf0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128355"
---
# <a name="list-childfolders"></a><span data-ttu-id="6c6d1-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="6c6d1-104">List childFolders</span></span>

<span data-ttu-id="6c6d1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c6d1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c6d1-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/mailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c6d1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c6d1-108">Permissions</span></span>

<span data-ttu-id="6c6d1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c6d1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c6d1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c6d1-111">Permission type</span></span>                        | <span data-ttu-id="6c6d1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c6d1-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="6c6d1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c6d1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c6d1-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c6d1-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="6c6d1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c6d1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c6d1-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c6d1-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="6c6d1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c6d1-117">Application</span></span>                            | <span data-ttu-id="6c6d1-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c6d1-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="6c6d1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c6d1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c6d1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6c6d1-120">Optional query parameters</span></span>

<span data-ttu-id="6c6d1-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c6d1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c6d1-122">Request headers</span></span>

| <span data-ttu-id="6c6d1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6c6d1-123">Name</span></span>          | <span data-ttu-id="6c6d1-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c6d1-124">Type</span></span>   | <span data-ttu-id="6c6d1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c6d1-125">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="6c6d1-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c6d1-126">Authorization</span></span> | <span data-ttu-id="6c6d1-127">string</span><span class="sxs-lookup"><span data-stu-id="6c6d1-127">string</span></span> | <span data-ttu-id="6c6d1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c6d1-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c6d1-130">Request body</span></span>

<span data-ttu-id="6c6d1-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c6d1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c6d1-132">Response</span></span>

<span data-ttu-id="6c6d1-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailfolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-133">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c6d1-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6c6d1-134">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="6c6d1-135">Exemplo 1: Listar pastas de email</span><span class="sxs-lookup"><span data-stu-id="6c6d1-135">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="6c6d1-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c6d1-136">Request</span></span>

<span data-ttu-id="6c6d1-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6c6d1-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c6d1-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="c"></a>[<span data-ttu-id="6c6d1-139">C#</span><span class="sxs-lookup"><span data-stu-id="6c6d1-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c6d1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c6d1-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c6d1-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c6d1-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c6d1-142">Java</span><span class="sxs-lookup"><span data-stu-id="6c6d1-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="6c6d1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c6d1-143">Response</span></span>

<span data-ttu-id="6c6d1-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-144">The following is an example of the response.</span></span>

> <span data-ttu-id="6c6d1-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="6c6d1-147">Exemplo 2: Listar pastas de pesquisa de email</span><span class="sxs-lookup"><span data-stu-id="6c6d1-147">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="6c6d1-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c6d1-148">Request</span></span>

<span data-ttu-id="6c6d1-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-149">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6c6d1-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c6d1-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="c"></a>[<span data-ttu-id="6c6d1-151">C#</span><span class="sxs-lookup"><span data-stu-id="6c6d1-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c6d1-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c6d1-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c6d1-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c6d1-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c6d1-154">Java</span><span class="sxs-lookup"><span data-stu-id="6c6d1-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-childfolders-of-searchfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c6d1-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c6d1-155">Response</span></span>

<span data-ttu-id="6c6d1-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-156">The following is an example of the response.</span></span>

> <span data-ttu-id="6c6d1-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c6d1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


