---
title: Obter contactFolder
description: Obtenha uma pasta de contatos usando a respectiva ID.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b5de49776c57789e04dd40723c4eb4f20ac03661
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417967"
---
# <a name="get-contactfolder"></a><span data-ttu-id="44db5-103">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="44db5-103">Get contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44db5-104">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="44db5-104">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="44db5-105">Há dois cenários em que um aplicativo pode obter a pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="44db5-105">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="44db5-106">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="44db5-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="44db5-107">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="44db5-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="44db5-108">Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="44db5-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="44db5-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="44db5-109">Permissions</span></span>
<span data-ttu-id="44db5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44db5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44db5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44db5-112">Permission type</span></span>      | <span data-ttu-id="44db5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44db5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44db5-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44db5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="44db5-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44db5-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="44db5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44db5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44db5-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44db5-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="44db5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44db5-118">Application</span></span> | <span data-ttu-id="44db5-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44db5-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="44db5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44db5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="44db5-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="44db5-121">Optional query parameters</span></span>
<span data-ttu-id="44db5-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="44db5-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="44db5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44db5-123">Request headers</span></span>
| <span data-ttu-id="44db5-124">Nome</span><span class="sxs-lookup"><span data-stu-id="44db5-124">Name</span></span>       | <span data-ttu-id="44db5-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="44db5-125">Type</span></span> | <span data-ttu-id="44db5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="44db5-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44db5-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="44db5-127">Authorization</span></span>  | <span data-ttu-id="44db5-128">string</span><span class="sxs-lookup"><span data-stu-id="44db5-128">string</span></span>  | <span data-ttu-id="44db5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44db5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44db5-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44db5-131">Request body</span></span>
<span data-ttu-id="44db5-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="44db5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44db5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="44db5-133">Response</span></span>

<span data-ttu-id="44db5-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44db5-134">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44db5-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44db5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44db5-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44db5-136">Request</span></span>
<span data-ttu-id="44db5-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44db5-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="44db5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="44db5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44db5-139">C#</span><span class="sxs-lookup"><span data-stu-id="44db5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44db5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44db5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44db5-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="44db5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44db5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="44db5-142">Response</span></span>
<span data-ttu-id="44db5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44db5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
