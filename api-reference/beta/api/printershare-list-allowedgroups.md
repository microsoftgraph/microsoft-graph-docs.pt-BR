---
title: Listar allowedGroups para printerShare
description: Recupere uma lista de grupos que tiveram acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 0a15472fd7935dc3eacc38c0a34a6e7a5c0eaf67
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766270"
---
# <a name="list-allowedgroups-for-printershare"></a><span data-ttu-id="4a44d-103">Listar allowedGroups para printerShare</span><span class="sxs-lookup"><span data-stu-id="4a44d-103">List allowedGroups for printerShare</span></span>

<span data-ttu-id="4a44d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a44d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a44d-105">Recupere uma lista de grupos que tiveram acesso para enviar trabalhos de impressão para a [impressora associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="4a44d-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a44d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a44d-106">Permissions</span></span>
<span data-ttu-id="4a44d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a44d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4a44d-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda acesso a [grupos de](group-list.md) lista.</span><span class="sxs-lookup"><span data-stu-id="4a44d-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List groups](group-list.md) access.</span></span> <span data-ttu-id="4a44d-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="4a44d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="4a44d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a44d-111">Permission type</span></span> | <span data-ttu-id="4a44d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a44d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4a44d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a44d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4a44d-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a44d-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="4a44d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a44d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a44d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a44d-116">Not Supported.</span></span>|
|<span data-ttu-id="4a44d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a44d-117">Application</span></span>|<span data-ttu-id="4a44d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a44d-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a44d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a44d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="4a44d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a44d-120">Request headers</span></span>
| <span data-ttu-id="4a44d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4a44d-121">Name</span></span>      |<span data-ttu-id="4a44d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a44d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a44d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a44d-123">Authorization</span></span> | <span data-ttu-id="4a44d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a44d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a44d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a44d-126">Request body</span></span>
<span data-ttu-id="4a44d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a44d-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4a44d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a44d-128">Response</span></span>
<span data-ttu-id="4a44d-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/group.md) grupo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a44d-129">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a44d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a44d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a44d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a44d-131">Request</span></span>
<span data-ttu-id="4a44d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a44d-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a44d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a44d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="4a44d-134">C#</span><span class="sxs-lookup"><span data-stu-id="4a44d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a44d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a44d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a44d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a44d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a44d-137">Java</span><span class="sxs-lookup"><span data-stu-id="4a44d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allowedgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a44d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a44d-138">Response</span></span>
<span data-ttu-id="4a44d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a44d-139">The following is an example of the response.</span></span>
><span data-ttu-id="4a44d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a44d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.group)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "GroupName"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
