---
title: Criar um permitido para printerShare
description: Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 21842b0d770991928e5d191cb4bed2335fc6fbcd
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372725"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="28665-103">Criar um permitido para printerShare</span><span class="sxs-lookup"><span data-stu-id="28665-103">Create allowedGroup for printerShare</span></span>

<span data-ttu-id="28665-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28665-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28665-105">Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="28665-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="28665-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28665-106">Permissions</span></span>
<span data-ttu-id="28665-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="28665-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="28665-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="28665-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="28665-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="28665-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28665-111">Permission type</span></span> | <span data-ttu-id="28665-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28665-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="28665-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28665-113">Delegated (work or school account)</span></span>| <span data-ttu-id="28665-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28665-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="28665-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28665-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28665-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28665-116">Not Supported.</span></span>|
|<span data-ttu-id="28665-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28665-117">Application</span></span>|<span data-ttu-id="28665-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28665-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28665-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28665-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="28665-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28665-120">Request headers</span></span>
| <span data-ttu-id="28665-121">Nome</span><span class="sxs-lookup"><span data-stu-id="28665-121">Name</span></span>          | <span data-ttu-id="28665-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="28665-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="28665-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="28665-123">Authorization</span></span> | <span data-ttu-id="28665-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28665-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28665-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="28665-126">Content-type</span></span>  | <span data-ttu-id="28665-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28665-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28665-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28665-129">Request body</span></span>
<span data-ttu-id="28665-130">No corpo da solicitação, forneça uma referência a uma entidade de grupo usando o `@odata.id` formato, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="28665-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="28665-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="28665-131">Response</span></span>
<span data-ttu-id="28665-132">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="28665-132">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="28665-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28665-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="28665-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28665-134">Request</span></span>
<span data-ttu-id="28665-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28665-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="28665-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="28665-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="28665-137">C#</span><span class="sxs-lookup"><span data-stu-id="28665-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-allowedgroup-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28665-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28665-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-allowedgroup-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28665-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28665-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-allowedgroup-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="28665-140">No corpo da solicitação, forneça uma referência a uma entidade de grupo incluindo o URI do Microsoft Graph do grupo no `@odata.id` campo do corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="28665-140">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="28665-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="28665-141">Response</span></span>
<span data-ttu-id="28665-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28665-142">The following is an example of the response.</span></span> 
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
