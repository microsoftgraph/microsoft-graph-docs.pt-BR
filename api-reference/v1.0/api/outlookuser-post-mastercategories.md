---
title: Criar categoria do Outlook
description: Cria um objeto outlookCategory na lista mestra de categorias do usuário.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0117b075dae4e7e38572781526fdc4e369f4d2fc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055859"
---
# <a name="create-outlook-category"></a><span data-ttu-id="c3b04-103">Criar categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="c3b04-103">Create Outlook category</span></span>

<span data-ttu-id="c3b04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3b04-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="c3b04-105">Cria um objeto [outlookCategory](../resources/outlookcategory.md) na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3b04-105">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3b04-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3b04-106">Permissions</span></span>
<span data-ttu-id="c3b04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3b04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3b04-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3b04-109">Permission type</span></span>      | <span data-ttu-id="c3b04-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3b04-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3b04-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3b04-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3b04-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3b04-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c3b04-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3b04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3b04-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3b04-114">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="c3b04-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3b04-115">Application</span></span> | <span data-ttu-id="c3b04-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3b04-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3b04-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3b04-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="c3b04-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3b04-118">Request headers</span></span>
| <span data-ttu-id="c3b04-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c3b04-119">Name</span></span>       | <span data-ttu-id="c3b04-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3b04-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c3b04-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3b04-121">Authorization</span></span>  | <span data-ttu-id="c3b04-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3b04-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c3b04-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3b04-124">Request body</span></span>
<span data-ttu-id="c3b04-125">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="c3b04-125">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c3b04-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3b04-126">Response</span></span>

<span data-ttu-id="c3b04-127">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3b04-127">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3b04-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3b04-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3b04-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3b04-129">Request</span></span>
<span data-ttu-id="c3b04-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3b04-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c3b04-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3b04-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
# <a name="c"></a>[<span data-ttu-id="c3b04-132">C#</span><span class="sxs-lookup"><span data-stu-id="c3b04-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlookcategory-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3b04-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3b04-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlookcategory-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3b04-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3b04-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlookcategory-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3b04-135">Java</span><span class="sxs-lookup"><span data-stu-id="c3b04-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlookcategory-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c3b04-136">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="c3b04-136">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c3b04-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3b04-137">Response</span></span>
<span data-ttu-id="c3b04-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3b04-138">Here is an example of the response.</span></span> <span data-ttu-id="c3b04-139">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c3b04-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

