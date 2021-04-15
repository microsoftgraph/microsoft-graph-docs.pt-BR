---
title: Listar allowedUsers for printerShare
description: Recupere uma lista de usuários que tiveram acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d66ba6d7d9eadecc4b6b1dc2346fbf6afe1e7378
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766004"
---
# <a name="list-allowedusers-for-printershare"></a><span data-ttu-id="57f73-103">Listar allowedUsers for printerShare</span><span class="sxs-lookup"><span data-stu-id="57f73-103">List allowedUsers for printerShare</span></span>

<span data-ttu-id="57f73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57f73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57f73-105">Recupere uma lista de usuários que tiveram acesso para enviar trabalhos de impressão para a [impressora associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="57f73-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="57f73-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="57f73-106">Permissions</span></span>
<span data-ttu-id="57f73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57f73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="57f73-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda acesso aos usuários [de](user-list.md) lista.</span><span class="sxs-lookup"><span data-stu-id="57f73-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List users](user-list.md) access.</span></span> <span data-ttu-id="57f73-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="57f73-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="57f73-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57f73-111">Permission type</span></span> | <span data-ttu-id="57f73-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57f73-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="57f73-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57f73-113">Delegated (work or school account)</span></span>| <span data-ttu-id="57f73-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57f73-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="57f73-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57f73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57f73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57f73-116">Not Supported.</span></span>|
|<span data-ttu-id="57f73-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57f73-117">Application</span></span>|<span data-ttu-id="57f73-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57f73-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57f73-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57f73-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="57f73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57f73-120">Request headers</span></span>
| <span data-ttu-id="57f73-121">Nome</span><span class="sxs-lookup"><span data-stu-id="57f73-121">Name</span></span>      |<span data-ttu-id="57f73-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="57f73-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57f73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57f73-123">Authorization</span></span> | <span data-ttu-id="57f73-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57f73-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57f73-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57f73-126">Request body</span></span>
<span data-ttu-id="57f73-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57f73-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="57f73-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="57f73-128">Response</span></span>
<span data-ttu-id="57f73-129">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57f73-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="57f73-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57f73-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="57f73-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57f73-131">Request</span></span>
<span data-ttu-id="57f73-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="57f73-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="57f73-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="57f73-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="57f73-134">C#</span><span class="sxs-lookup"><span data-stu-id="57f73-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57f73-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57f73-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57f73-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57f73-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57f73-137">Java</span><span class="sxs-lookup"><span data-stu-id="57f73-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allowedusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57f73-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="57f73-138">Response</span></span>
<span data-ttu-id="57f73-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="57f73-139">The following is an example of the response.</span></span>
><span data-ttu-id="57f73-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57f73-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 286

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.user)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
