---
title: Criar um permitido
description: Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 22512c6de88d85c09c0924fbc66eef9b760c6ce0
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216802"
---
# <a name="create-allowedgroup"></a><span data-ttu-id="7200a-103">Criar um permitido</span><span class="sxs-lookup"><span data-stu-id="7200a-103">Create allowedGroup</span></span>

<span data-ttu-id="7200a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7200a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7200a-105">Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="7200a-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7200a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7200a-106">Permissions</span></span>
<span data-ttu-id="7200a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7200a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7200a-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="7200a-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="7200a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7200a-110">Permission type</span></span> | <span data-ttu-id="7200a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7200a-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7200a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7200a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="7200a-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="7200a-113">Users.Read.All</span></span> |
|<span data-ttu-id="7200a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7200a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7200a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7200a-115">Not Supported.</span></span>|
|<span data-ttu-id="7200a-116">Application</span><span class="sxs-lookup"><span data-stu-id="7200a-116">Application</span></span>|<span data-ttu-id="7200a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7200a-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7200a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7200a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7200a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7200a-119">Request headers</span></span>
| <span data-ttu-id="7200a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7200a-120">Name</span></span>          | <span data-ttu-id="7200a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7200a-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7200a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7200a-122">Authorization</span></span> | <span data-ttu-id="7200a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7200a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7200a-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="7200a-125">Content-type</span></span>  | <span data-ttu-id="7200a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7200a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7200a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7200a-128">Request body</span></span>
<span data-ttu-id="7200a-129">No corpo da solicitação, forneça uma referência a uma entidade de grupo usando o `@odata.id` formato, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="7200a-129">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="7200a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7200a-130">Response</span></span>
<span data-ttu-id="7200a-131">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="7200a-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7200a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7200a-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="7200a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7200a-133">Request</span></span>
<span data-ttu-id="7200a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7200a-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7200a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7200a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_allowedgroup_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups/$ref
Content-type: application/json
Content-length: 67

{
  "@odata.id": "https://graph.microsoft.com/beta/groups/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="7200a-136">C#</span><span class="sxs-lookup"><span data-stu-id="7200a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-allowedgroup-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7200a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7200a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-allowedgroup-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7200a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7200a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-allowedgroup-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="7200a-139">No corpo da solicitação, forneça uma referência a uma entidade de grupo incluindo o URI do Microsoft Graph do grupo no `@odata.id` campo do corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="7200a-139">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="7200a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7200a-140">Response</span></span>
<span data-ttu-id="7200a-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7200a-141">The following is an example of the response.</span></span> 
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
  "description": "Create allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
