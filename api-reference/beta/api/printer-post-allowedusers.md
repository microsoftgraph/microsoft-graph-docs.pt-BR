---
title: Criar allowedUser
description: Conceda ao usuário especificado acesso para enviar trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5ce2564b2878a3dff998c938366f132c08098a73
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947795"
---
# <a name="create-alloweduser"></a><span data-ttu-id="4ef49-103">Criar allowedUser</span><span class="sxs-lookup"><span data-stu-id="4ef49-103">Create allowedUser</span></span>

<span data-ttu-id="4ef49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ef49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ef49-105">Conceda ao usuário especificado acesso para enviar **trabalhos de impressão** à [impressora](../resources/printer.md)associada.</span><span class="sxs-lookup"><span data-stu-id="4ef49-105">Grant the specified user access to submit **print jobs** to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ef49-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ef49-106">Permissions</span></span>
<span data-ttu-id="4ef49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ef49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4ef49-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="4ef49-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4ef49-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ef49-110">Permission type</span></span> | <span data-ttu-id="4ef49-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ef49-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4ef49-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ef49-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4ef49-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="4ef49-113">Users.Read.All</span></span> |
|<span data-ttu-id="4ef49-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ef49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ef49-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ef49-115">Not Supported.</span></span>|
|<span data-ttu-id="4ef49-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ef49-116">Application</span></span>|<span data-ttu-id="4ef49-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ef49-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ef49-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ef49-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/allowedUsers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4ef49-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ef49-119">Request headers</span></span>
| <span data-ttu-id="4ef49-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4ef49-120">Name</span></span>          | <span data-ttu-id="4ef49-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ef49-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4ef49-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ef49-122">Authorization</span></span> | <span data-ttu-id="4ef49-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ef49-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ef49-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="4ef49-125">Content-type</span></span>  | <span data-ttu-id="4ef49-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ef49-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ef49-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ef49-128">Request body</span></span>
<span data-ttu-id="4ef49-129">No corpo da solicitação, forneça uma referência a uma entidade de usuário usando o `@odata.id` formato, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4ef49-129">In the request body, supply a reference to a user entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="4ef49-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ef49-130">Response</span></span>
<span data-ttu-id="4ef49-131">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="4ef49-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4ef49-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ef49-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ef49-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ef49-133">Request</span></span>
<span data-ttu-id="4ef49-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ef49-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ef49-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ef49-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_alloweduser_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/allowedUsers/$ref
Content-type: application/json
Content-length: 66

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="4ef49-136">C#</span><span class="sxs-lookup"><span data-stu-id="4ef49-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-alloweduser-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ef49-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ef49-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-alloweduser-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ef49-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ef49-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-alloweduser-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4ef49-139">No corpo da solicitação, forneça uma referência a uma entidade de usuário, incluindo o URI do Microsoft Graph do usuário `@odata.id` no campo do corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef49-139">In the request body, supply a reference to a user entity by including the user's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

##### <a name="response"></a><span data-ttu-id="4ef49-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ef49-140">Response</span></span>
<span data-ttu-id="4ef49-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ef49-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
