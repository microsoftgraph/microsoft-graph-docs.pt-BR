---
title: Criar allowedGroup para printerShare
description: Conceda ao grupo especificado acesso para enviar trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1b6e11b1f4a650755d696e5bc346f4cf369324bb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787524"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="3c080-103">Criar allowedGroup para printerShare</span><span class="sxs-lookup"><span data-stu-id="3c080-103">Create allowedGroup for printerShare</span></span>

<span data-ttu-id="3c080-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c080-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c080-105">Conceda ao grupo especificado acesso para enviar trabalhos de impressão para a [impressora associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="3c080-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c080-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3c080-106">Permissions</span></span>
<span data-ttu-id="3c080-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3c080-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="3c080-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="3c080-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="3c080-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="3c080-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c080-111">Permission type</span></span> | <span data-ttu-id="3c080-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c080-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3c080-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c080-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3c080-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c080-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="3c080-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c080-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c080-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c080-116">Not Supported.</span></span>|
|<span data-ttu-id="3c080-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c080-117">Application</span></span>|<span data-ttu-id="3c080-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c080-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c080-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c080-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="3c080-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c080-120">Request headers</span></span>
| <span data-ttu-id="3c080-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3c080-121">Name</span></span>          | <span data-ttu-id="3c080-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c080-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3c080-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c080-123">Authorization</span></span> | <span data-ttu-id="3c080-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c080-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c080-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="3c080-126">Content-type</span></span>  | <span data-ttu-id="3c080-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c080-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c080-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c080-129">Request body</span></span>
<span data-ttu-id="3c080-130">No corpo da solicitação, fornece uma referência a uma entidade de grupo usando o formato, conforme `@odata.id` mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="3c080-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="3c080-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c080-131">Response</span></span>
<span data-ttu-id="3c080-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3c080-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3c080-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c080-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c080-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c080-134">Request</span></span>
<span data-ttu-id="3c080-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c080-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3c080-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c080-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3c080-137">C#</span><span class="sxs-lookup"><span data-stu-id="3c080-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-allowedgroup-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c080-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c080-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-allowedgroup-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c080-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c080-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-allowedgroup-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c080-140">Java</span><span class="sxs-lookup"><span data-stu-id="3c080-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-allowedgroup-from-printers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3c080-141">No corpo da solicitação, fornece uma referência a uma entidade de grupo incluindo o URI microsoft Graph do grupo no campo `@odata.id` do corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="3c080-141">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="3c080-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c080-142">Response</span></span>
<span data-ttu-id="3c080-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c080-143">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
