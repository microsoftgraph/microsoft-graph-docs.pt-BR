---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para acessar o nível superior '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 00a50cb94dd519d83899a201d710089eb47dc411
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812842"
---
# <a name="list-childfolders"></a><span data-ttu-id="24a7c-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="24a7c-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24a7c-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/mailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="24a7c-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="24a7c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="24a7c-107">Permissions</span></span>

<span data-ttu-id="24a7c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24a7c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24a7c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24a7c-110">Permission type</span></span>                        | <span data-ttu-id="24a7c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24a7c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="24a7c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24a7c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="24a7c-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24a7c-113">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="24a7c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24a7c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24a7c-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24a7c-115">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="24a7c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24a7c-116">Application</span></span>                            | <span data-ttu-id="24a7c-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24a7c-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="24a7c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24a7c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24a7c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24a7c-119">Optional query parameters</span></span>

<span data-ttu-id="24a7c-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24a7c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24a7c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24a7c-121">Request headers</span></span>

| <span data-ttu-id="24a7c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="24a7c-122">Name</span></span>          | <span data-ttu-id="24a7c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="24a7c-123">Type</span></span>   | <span data-ttu-id="24a7c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="24a7c-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="24a7c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="24a7c-125">Authorization</span></span> | <span data-ttu-id="24a7c-126">string</span><span class="sxs-lookup"><span data-stu-id="24a7c-126">string</span></span> | <span data-ttu-id="24a7c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24a7c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24a7c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24a7c-129">Request body</span></span>

<span data-ttu-id="24a7c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24a7c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24a7c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="24a7c-131">Response</span></span>

<span data-ttu-id="24a7c-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24a7c-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24a7c-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="24a7c-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="24a7c-134">Exemplo 1: listar pastas de email</span><span class="sxs-lookup"><span data-stu-id="24a7c-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="24a7c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24a7c-135">Request</span></span>

<span data-ttu-id="24a7c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="24a7c-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="24a7c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="24a7c-137">Response</span></span>

<span data-ttu-id="24a7c-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="24a7c-138">The following is an example of the response.</span></span>

> <span data-ttu-id="24a7c-139">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24a7c-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="24a7c-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24a7c-140">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="24a7c-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="24a7c-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="24a7c-142">C#</span><span class="sxs-lookup"><span data-stu-id="24a7c-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24a7c-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="24a7c-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="24a7c-144">Exemplo 2: listar pastas de pesquisa de email</span><span class="sxs-lookup"><span data-stu-id="24a7c-144">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="24a7c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24a7c-145">Request</span></span>

<span data-ttu-id="24a7c-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="24a7c-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="24a7c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="24a7c-147">Response</span></span>

<span data-ttu-id="24a7c-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="24a7c-148">The following is an example of the response.</span></span>

> <span data-ttu-id="24a7c-149">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24a7c-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="24a7c-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24a7c-150">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="24a7c-151">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="24a7c-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="24a7c-152">C#</span><span class="sxs-lookup"><span data-stu-id="24a7c-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24a7c-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="24a7c-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
