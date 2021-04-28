---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para acessar o nível superior '
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9080d3ac5cc8cc027386c1bcb740f7f084689abe
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055950"
---
# <a name="list-childfolders"></a><span data-ttu-id="f6a1a-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="f6a1a-104">List childFolders</span></span>

<span data-ttu-id="f6a1a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6a1a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6a1a-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/mailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="f6a1a-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6a1a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6a1a-108">Permissions</span></span>
<span data-ttu-id="f6a1a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6a1a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6a1a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6a1a-111">Permission type</span></span>      | <span data-ttu-id="f6a1a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6a1a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6a1a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6a1a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f6a1a-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6a1a-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6a1a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6a1a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6a1a-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6a1a-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6a1a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6a1a-117">Application</span></span> | <span data-ttu-id="f6a1a-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6a1a-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6a1a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6a1a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6a1a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6a1a-120">Optional query parameters</span></span>
<span data-ttu-id="f6a1a-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f6a1a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f6a1a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6a1a-122">Request headers</span></span>
| <span data-ttu-id="f6a1a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f6a1a-123">Name</span></span>       | <span data-ttu-id="f6a1a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6a1a-124">Type</span></span> | <span data-ttu-id="f6a1a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6a1a-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f6a1a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6a1a-126">Authorization</span></span>  | <span data-ttu-id="f6a1a-127">string</span><span class="sxs-lookup"><span data-stu-id="f6a1a-127">string</span></span>  | <span data-ttu-id="f6a1a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6a1a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6a1a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6a1a-130">Request body</span></span>
<span data-ttu-id="f6a1a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6a1a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6a1a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6a1a-132">Response</span></span>

<span data-ttu-id="f6a1a-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailfolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6a1a-133">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6a1a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6a1a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6a1a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6a1a-135">Request</span></span>
<span data-ttu-id="f6a1a-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6a1a-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6a1a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6a1a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="f6a1a-138">C#</span><span class="sxs-lookup"><span data-stu-id="f6a1a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6a1a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6a1a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6a1a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6a1a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6a1a-141">Java</span><span class="sxs-lookup"><span data-stu-id="f6a1a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f6a1a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6a1a-142">Response</span></span>
<span data-ttu-id="f6a1a-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6a1a-143">Here is an example of the response.</span></span> <span data-ttu-id="f6a1a-144">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f6a1a-144">Note: The response object shown here might be shortened for readability.</span></span>
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
