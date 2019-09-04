---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para acessar o nível superior '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1dbf07465c84538ef18dc94bf9ba59e615d89b34
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728727"
---
# <a name="list-childfolders"></a><span data-ttu-id="3c7c7-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="3c7c7-104">List childFolders</span></span>

<span data-ttu-id="3c7c7-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/mailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="3c7c7-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c7c7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c7c7-107">Permissions</span></span>
<span data-ttu-id="3c7c7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c7c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c7c7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c7c7-110">Permission type</span></span>      | <span data-ttu-id="3c7c7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c7c7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c7c7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c7c7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c7c7-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c7c7-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3c7c7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c7c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c7c7-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c7c7-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3c7c7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c7c7-116">Application</span></span> | <span data-ttu-id="3c7c7-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c7c7-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c7c7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c7c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c7c7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c7c7-119">Optional query parameters</span></span>
<span data-ttu-id="3c7c7-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c7c7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3c7c7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c7c7-121">Request headers</span></span>
| <span data-ttu-id="3c7c7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3c7c7-122">Name</span></span>       | <span data-ttu-id="3c7c7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c7c7-123">Type</span></span> | <span data-ttu-id="3c7c7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c7c7-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c7c7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c7c7-125">Authorization</span></span>  | <span data-ttu-id="3c7c7-126">string</span><span class="sxs-lookup"><span data-stu-id="3c7c7-126">string</span></span>  | <span data-ttu-id="3c7c7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c7c7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c7c7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c7c7-129">Request body</span></span>
<span data-ttu-id="3c7c7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c7c7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c7c7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c7c7-131">Response</span></span>

<span data-ttu-id="3c7c7-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailfolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c7c7-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c7c7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c7c7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c7c7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c7c7-134">Request</span></span>
<span data-ttu-id="3c7c7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c7c7-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3c7c7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c7c7-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c7c7-137">C#</span><span class="sxs-lookup"><span data-stu-id="3c7c7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c7c7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c7c7-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c7c7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c7c7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3c7c7-140">Java</span><span class="sxs-lookup"><span data-stu-id="3c7c7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c7c7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c7c7-141">Response</span></span>
<span data-ttu-id="3c7c7-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c7c7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
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
