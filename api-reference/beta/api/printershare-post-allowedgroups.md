---
title: Criar um permitido para printerShare
description: Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 0d1217c43b88803645fa1c4013a53691941717cc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967781"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="999ff-103">Criar um permitido para printerShare</span><span class="sxs-lookup"><span data-stu-id="999ff-103">Create allowedGroup for printerShare</span></span>

<span data-ttu-id="999ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="999ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="999ff-105">Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="999ff-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="999ff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="999ff-106">Permissions</span></span>
<span data-ttu-id="999ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="999ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="999ff-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="999ff-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="999ff-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="999ff-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="999ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="999ff-111">Permission type</span></span> | <span data-ttu-id="999ff-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="999ff-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="999ff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="999ff-113">Delegated (work or school account)</span></span>| <span data-ttu-id="999ff-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="999ff-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="999ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="999ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="999ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="999ff-116">Not Supported.</span></span>|
|<span data-ttu-id="999ff-117">Application</span><span class="sxs-lookup"><span data-stu-id="999ff-117">Application</span></span>|<span data-ttu-id="999ff-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="999ff-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="999ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="999ff-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="999ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="999ff-120">Request headers</span></span>
| <span data-ttu-id="999ff-121">Nome</span><span class="sxs-lookup"><span data-stu-id="999ff-121">Name</span></span>          | <span data-ttu-id="999ff-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="999ff-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="999ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="999ff-123">Authorization</span></span> | <span data-ttu-id="999ff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="999ff-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="999ff-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="999ff-126">Content-type</span></span>  | <span data-ttu-id="999ff-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="999ff-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="999ff-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="999ff-129">Request body</span></span>
<span data-ttu-id="999ff-130">No corpo da solicitação, forneça uma referência a uma entidade de grupo usando o `@odata.id` formato, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="999ff-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="999ff-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="999ff-131">Response</span></span>
<span data-ttu-id="999ff-132">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="999ff-132">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="999ff-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="999ff-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="999ff-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="999ff-134">Request</span></span>
<span data-ttu-id="999ff-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="999ff-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="999ff-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="999ff-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="999ff-137">C#</span><span class="sxs-lookup"><span data-stu-id="999ff-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-allowedgroup-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="999ff-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="999ff-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-allowedgroup-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="999ff-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="999ff-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-allowedgroup-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="999ff-140">Java</span><span class="sxs-lookup"><span data-stu-id="999ff-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-allowedgroup-from-printers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="999ff-141">No corpo da solicitação, forneça uma referência a uma entidade de grupo incluindo o URI do Microsoft Graph do grupo no `@odata.id` campo do corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="999ff-141">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="999ff-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="999ff-142">Response</span></span>
<span data-ttu-id="999ff-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="999ff-143">The following is an example of the response.</span></span> 
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
