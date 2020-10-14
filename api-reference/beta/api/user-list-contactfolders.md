---
title: Listar contactFolders
description: Obter todas as pastas de contatos na caixa de correio do usuário conectado.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f59362e627dc4b23be75f70b84e9824dd7f9ce16
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459505"
---
# <a name="list-contactfolders"></a><span data-ttu-id="a27b1-103">Listar contactFolders</span><span class="sxs-lookup"><span data-stu-id="a27b1-103">List contactFolders</span></span>

<span data-ttu-id="a27b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a27b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a27b1-105">Obter todas as pastas de contatos na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a27b1-105">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="a27b1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a27b1-106">Permissions</span></span>
<span data-ttu-id="a27b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a27b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a27b1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a27b1-109">Permission type</span></span>      | <span data-ttu-id="a27b1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a27b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a27b1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a27b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a27b1-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a27b1-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a27b1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a27b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a27b1-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a27b1-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a27b1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a27b1-115">Application</span></span> | <span data-ttu-id="a27b1-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a27b1-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a27b1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a27b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a27b1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a27b1-118">Optional query parameters</span></span>
<span data-ttu-id="a27b1-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a27b1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a27b1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a27b1-120">Request headers</span></span>
| <span data-ttu-id="a27b1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a27b1-121">Header</span></span>       | <span data-ttu-id="a27b1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a27b1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a27b1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a27b1-123">Authorization</span></span>  | <span data-ttu-id="a27b1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a27b1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a27b1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a27b1-126">Content-Type</span></span>   | <span data-ttu-id="a27b1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a27b1-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a27b1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a27b1-128">Request body</span></span>
<span data-ttu-id="a27b1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a27b1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a27b1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27b1-130">Response</span></span>

<span data-ttu-id="a27b1-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a27b1-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a27b1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a27b1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a27b1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a27b1-133">Request</span></span>
<span data-ttu-id="a27b1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a27b1-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a27b1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a27b1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders
```
# <a name="c"></a>[<span data-ttu-id="a27b1-136">C#</span><span class="sxs-lookup"><span data-stu-id="a27b1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a27b1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a27b1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a27b1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a27b1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a27b1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27b1-139">Response</span></span>
<span data-ttu-id="a27b1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a27b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
