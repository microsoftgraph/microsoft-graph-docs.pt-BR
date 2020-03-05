---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para acessar o nível superior '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ec9b2e89dacf80c24c9036ed0d8d932856eac4d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457049"
---
# <a name="list-childfolders"></a><span data-ttu-id="b6d97-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="b6d97-104">List childFolders</span></span>

<span data-ttu-id="b6d97-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6d97-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6d97-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/mailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="b6d97-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6d97-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6d97-108">Permissions</span></span>

<span data-ttu-id="b6d97-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6d97-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6d97-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6d97-111">Permission type</span></span>                        | <span data-ttu-id="b6d97-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6d97-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="b6d97-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6d97-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6d97-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6d97-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="b6d97-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6d97-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6d97-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6d97-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="b6d97-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6d97-117">Application</span></span>                            | <span data-ttu-id="b6d97-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6d97-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="b6d97-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6d97-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6d97-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6d97-120">Optional query parameters</span></span>

<span data-ttu-id="b6d97-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6d97-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6d97-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d97-122">Request headers</span></span>

| <span data-ttu-id="b6d97-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b6d97-123">Name</span></span>          | <span data-ttu-id="b6d97-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6d97-124">Type</span></span>   | <span data-ttu-id="b6d97-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d97-125">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="b6d97-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6d97-126">Authorization</span></span> | <span data-ttu-id="b6d97-127">string</span><span class="sxs-lookup"><span data-stu-id="b6d97-127">string</span></span> | <span data-ttu-id="b6d97-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6d97-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6d97-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d97-130">Request body</span></span>

<span data-ttu-id="b6d97-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6d97-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6d97-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6d97-132">Response</span></span>

<span data-ttu-id="b6d97-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailfolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6d97-133">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6d97-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b6d97-134">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="b6d97-135">Exemplo 1: listar pastas de email</span><span class="sxs-lookup"><span data-stu-id="b6d97-135">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="b6d97-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d97-136">Request</span></span>

<span data-ttu-id="b6d97-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6d97-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b6d97-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6d97-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="c"></a>[<span data-ttu-id="b6d97-139">C#</span><span class="sxs-lookup"><span data-stu-id="b6d97-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6d97-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6d97-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6d97-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6d97-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="b6d97-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6d97-142">Response</span></span>

<span data-ttu-id="b6d97-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6d97-143">The following is an example of the response.</span></span>

> <span data-ttu-id="b6d97-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6d97-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6d97-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6d97-145">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="b6d97-146">Exemplo 2: listar pastas de pesquisa de email</span><span class="sxs-lookup"><span data-stu-id="b6d97-146">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="b6d97-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d97-147">Request</span></span>

<span data-ttu-id="b6d97-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6d97-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b6d97-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6d97-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="c"></a>[<span data-ttu-id="b6d97-150">C#</span><span class="sxs-lookup"><span data-stu-id="b6d97-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6d97-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6d97-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6d97-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6d97-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b6d97-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6d97-153">Response</span></span>

<span data-ttu-id="b6d97-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6d97-154">The following is an example of the response.</span></span>

> <span data-ttu-id="b6d97-155">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6d97-155">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6d97-156">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6d97-156">All the properties will be returned from an actual call.</span></span>

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
