---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para chegar o nível superior '
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c3b589db36b645884ec5218ef25b9c56949fbaf5
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629445"
---
# <a name="list-childfolders"></a><span data-ttu-id="807f2-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="807f2-104">List childFolders</span></span>

<span data-ttu-id="807f2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="807f2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="807f2-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/mailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="807f2-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

<span data-ttu-id="807f2-108">Por padrão, esta operação não retorna pastas ocultas.</span><span class="sxs-lookup"><span data-stu-id="807f2-108">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="807f2-109">Use um parâmetro de consulta _includeHiddenFolders_ para incluí-los na resposta.</span><span class="sxs-lookup"><span data-stu-id="807f2-109">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="807f2-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="807f2-110">Permissions</span></span>
<span data-ttu-id="807f2-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="807f2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="807f2-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="807f2-113">Permission type</span></span>      | <span data-ttu-id="807f2-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="807f2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="807f2-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="807f2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="807f2-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="807f2-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="807f2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="807f2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="807f2-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="807f2-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="807f2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="807f2-119">Application</span></span> | <span data-ttu-id="807f2-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="807f2-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="807f2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="807f2-121">HTTP request</span></span>

<span data-ttu-id="807f2-122">Para obter todas as pastas filho na pasta especificada, excluindo aquelas que estão ocultas:</span><span class="sxs-lookup"><span data-stu-id="807f2-122">To get all the child folders under the specified folder, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="807f2-123">Para incluir pastas filho _ocultas_ na resposta:</span><span class="sxs-lookup"><span data-stu-id="807f2-123">To include _hidden_ child folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="807f2-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="807f2-124">Optional query parameters</span></span>
<span data-ttu-id="807f2-125">Para retornar uma lista de todas as childFolders incluindo aquelas que estão ocultas (sua propriedade **isHidden** é verdadeira), no URL de solicitação, especifique o `includeHiddenFolders` parâmetro de consulta como `true`, conforme mostrado na seção de [solicitação HTTP](#http-request).</span><span class="sxs-lookup"><span data-stu-id="807f2-125">To return a list of all childFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="807f2-126">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="807f2-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="807f2-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="807f2-127">Request headers</span></span>
| <span data-ttu-id="807f2-128">Nome</span><span class="sxs-lookup"><span data-stu-id="807f2-128">Name</span></span>       | <span data-ttu-id="807f2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="807f2-129">Type</span></span> | <span data-ttu-id="807f2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="807f2-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="807f2-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="807f2-131">Authorization</span></span>  | <span data-ttu-id="807f2-132">string</span><span class="sxs-lookup"><span data-stu-id="807f2-132">string</span></span>  | <span data-ttu-id="807f2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="807f2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="807f2-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="807f2-135">Request body</span></span>
<span data-ttu-id="807f2-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="807f2-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="807f2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="807f2-137">Response</span></span>

<span data-ttu-id="807f2-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailfolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="807f2-138">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="807f2-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="807f2-139">Example</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="807f2-140">Exemplo 1: Lista de pastas de email</span><span class="sxs-lookup"><span data-stu-id="807f2-140">Example 1: List mail folders</span></span>

<span data-ttu-id="807f2-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="807f2-141">The following is an example of the request.</span></span>

##### <a name="request"></a><span data-ttu-id="807f2-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="807f2-142">Request</span></span>
<span data-ttu-id="807f2-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="807f2-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="807f2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="807f2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="807f2-145">C#</span><span class="sxs-lookup"><span data-stu-id="807f2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="807f2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="807f2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="807f2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="807f2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="807f2-148">Java</span><span class="sxs-lookup"><span data-stu-id="807f2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="807f2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="807f2-149">Response</span></span>
<span data-ttu-id="807f2-p106">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="807f2-p106">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "isHidden": false
    }
  ]
}
```
### <a name="example-2-include-hidden-child-folders-under-a-specified-mail-folder"></a><span data-ttu-id="807f2-152">Exemplo 2: Incluir pastas filho ocultas em uma pasta de email especificada</span><span class="sxs-lookup"><span data-stu-id="807f2-152">Example 2: Include hidden child folders under a specified mail folder</span></span>

<span data-ttu-id="807f2-153">O próximo exemplo usa o parâmetro de consulta `includeHiddenFolders` para obter uma lista de pastas filho em uma pasta de email especificada, incluindo pastas de email ocultas.</span><span class="sxs-lookup"><span data-stu-id="807f2-153">The next example uses the `includeHiddenFolders` query parameter to get a list of child folders under a specified mail folder including hidden mail folders.</span></span> <span data-ttu-id="807f2-154">A resposta inclui a pasta "Emails secundários" que tem a **isHidden** definida como verdadeira.</span><span class="sxs-lookup"><span data-stu-id="807f2-154">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

##### <a name="request"></a><span data-ttu-id="807f2-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="807f2-155">Request</span></span>
<span data-ttu-id="807f2-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="807f2-156">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "mailfolder_get_hiddenchildfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders?includeHiddenFolders=true
```

##### <a name="response"></a><span data-ttu-id="807f2-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="807f2-157">Response</span></span>
<span data-ttu-id="807f2-p108">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="807f2-p108">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "id": "AAMkAGVmMDEzA",
      "displayName": "Internal Screens",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 2,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Clutters",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "isHidden": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
