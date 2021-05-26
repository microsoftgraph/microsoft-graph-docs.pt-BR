---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para chegar o nível superior '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c42d214e9c099c8d732eb73b93d16b5392801138
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665243"
---
# <a name="list-childfolders"></a><span data-ttu-id="c33a1-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="c33a1-104">List childFolders</span></span>

<span data-ttu-id="c33a1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c33a1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c33a1-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/mailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="c33a1-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

<span data-ttu-id="c33a1-108">Por padrão, esta operação não retorna pastas ocultas.</span><span class="sxs-lookup"><span data-stu-id="c33a1-108">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="c33a1-109">Use um parâmetro de consulta _includeHiddenFolders_ para incluí-los na resposta.</span><span class="sxs-lookup"><span data-stu-id="c33a1-109">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="c33a1-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="c33a1-110">Permissions</span></span>

<span data-ttu-id="c33a1-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c33a1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c33a1-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c33a1-113">Permission type</span></span>                        | <span data-ttu-id="c33a1-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c33a1-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="c33a1-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c33a1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="c33a1-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c33a1-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="c33a1-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c33a1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c33a1-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c33a1-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="c33a1-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c33a1-119">Application</span></span>                            | <span data-ttu-id="c33a1-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c33a1-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="c33a1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c33a1-121">HTTP request</span></span>

<span data-ttu-id="c33a1-122">Para obter todas as pastas filho na pasta especificada, excluindo aquelas que estão ocultas:</span><span class="sxs-lookup"><span data-stu-id="c33a1-122">To get all the child folders under the specified folder, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="c33a1-123">Para incluir pastas filho _ocultas_ na resposta:</span><span class="sxs-lookup"><span data-stu-id="c33a1-123">To include _hidden_ child folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c33a1-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c33a1-124">Optional query parameters</span></span>
<span data-ttu-id="c33a1-125">Para retornar uma lista de todas as childFolders incluindo aquelas que estão ocultas (sua propriedade **isHidden** é verdadeira), no URL de solicitação, especifique o `includeHiddenFolders` parâmetro de consulta como `true`, conforme mostrado na seção de [solicitação HTTP](#http-request).</span><span class="sxs-lookup"><span data-stu-id="c33a1-125">To return a list of all childFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="c33a1-126">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c33a1-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c33a1-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c33a1-127">Request headers</span></span>

| <span data-ttu-id="c33a1-128">Nome</span><span class="sxs-lookup"><span data-stu-id="c33a1-128">Name</span></span>          | <span data-ttu-id="c33a1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c33a1-129">Type</span></span>   | <span data-ttu-id="c33a1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33a1-130">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="c33a1-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c33a1-131">Authorization</span></span> | <span data-ttu-id="c33a1-132">string</span><span class="sxs-lookup"><span data-stu-id="c33a1-132">string</span></span> | <span data-ttu-id="c33a1-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c33a1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c33a1-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c33a1-135">Request body</span></span>

<span data-ttu-id="c33a1-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c33a1-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c33a1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c33a1-137">Response</span></span>

<span data-ttu-id="c33a1-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailfolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c33a1-138">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c33a1-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c33a1-139">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="c33a1-140">Exemplo 1: Lista de pastas de email</span><span class="sxs-lookup"><span data-stu-id="c33a1-140">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="c33a1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c33a1-141">Request</span></span>

<span data-ttu-id="c33a1-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c33a1-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c33a1-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c33a1-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="c"></a>[<span data-ttu-id="c33a1-144">C#</span><span class="sxs-lookup"><span data-stu-id="c33a1-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c33a1-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c33a1-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c33a1-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c33a1-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c33a1-147">Java</span><span class="sxs-lookup"><span data-stu-id="c33a1-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c33a1-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c33a1-148">Response</span></span>

<span data-ttu-id="c33a1-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c33a1-149">The following is an example of the response.</span></span>

> <span data-ttu-id="c33a1-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c33a1-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "wellKnownName": null,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Project Falcon",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders",
      "isHidden": false
    }
  ]
}
```

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="c33a1-151">Exemplo 2: Listar pastas de pesquisa de email</span><span class="sxs-lookup"><span data-stu-id="c33a1-151">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="c33a1-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c33a1-152">Request</span></span>

<span data-ttu-id="c33a1-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c33a1-153">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c33a1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="c33a1-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="c"></a>[<span data-ttu-id="c33a1-155">C#</span><span class="sxs-lookup"><span data-stu-id="c33a1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c33a1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c33a1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c33a1-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c33a1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c33a1-158">Java</span><span class="sxs-lookup"><span data-stu-id="c33a1-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-childfolders-of-searchfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c33a1-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="c33a1-159">Response</span></span>

<span data-ttu-id="c33a1-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c33a1-160">The following is an example of the response.</span></span>

> <span data-ttu-id="c33a1-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c33a1-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "isHidden": false,
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
      "isHidden": false,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
    }
  ]
}
```

### <a name="example-3-include-hidden-child-folders-under-a-specified-mail-folder"></a><span data-ttu-id="c33a1-162">Exemplo 3: Incluir pastas filho ocultas em uma pasta de email especificada</span><span class="sxs-lookup"><span data-stu-id="c33a1-162">Example 3: Include hidden child folders under a specified mail folder</span></span>

<span data-ttu-id="c33a1-163">O próximo exemplo usa o parâmetro de consulta `includeHiddenFolders` para obter uma lista de pastas filho em uma pasta de email especificada, incluindo pastas de email ocultas.</span><span class="sxs-lookup"><span data-stu-id="c33a1-163">The next example uses the `includeHiddenFolders` query parameter to get a list of child folders under a specified mail folder including hidden mail folders.</span></span> <span data-ttu-id="c33a1-164">A resposta inclui a pasta "Emails secundários" que tem a **isHidden** definida como verdadeira.</span><span class="sxs-lookup"><span data-stu-id="c33a1-164">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="c33a1-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c33a1-165">Request</span></span>

<span data-ttu-id="c33a1-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c33a1-166">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="c33a1-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="c33a1-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_hiddenchildfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders?includeHiddenFolders=true
```
# <a name="c"></a>[<span data-ttu-id="c33a1-168">C#</span><span class="sxs-lookup"><span data-stu-id="c33a1-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-hiddenchildfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c33a1-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c33a1-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-hiddenchildfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c33a1-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c33a1-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-hiddenchildfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c33a1-171">Java</span><span class="sxs-lookup"><span data-stu-id="c33a1-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-hiddenchildfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c33a1-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="c33a1-172">Response</span></span>

<span data-ttu-id="c33a1-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c33a1-173">The following is an example of the response.</span></span>

> <span data-ttu-id="c33a1-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c33a1-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "wellKnownName": null,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Clutters",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null,
      "isHidden": true
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders",
      "isHidden": false
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


