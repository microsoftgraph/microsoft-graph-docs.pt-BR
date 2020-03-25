---
title: Listar allowedGroups
description: Recupere uma lista de grupos aos quais o acesso foi concedido para enviar trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c076026d709ff26e1e00def3262069b3b79165a7
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947916"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="4e2b7-103">Listar allowedGroups</span><span class="sxs-lookup"><span data-stu-id="4e2b7-103">List allowedGroups</span></span>

<span data-ttu-id="4e2b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e2b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e2b7-105">Recupere uma lista de grupos aos quais o acesso foi concedido para enviar trabalhos de impressão à [impressora](../resources/printer.md)associada.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e2b7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e2b7-106">Permissions</span></span>
<span data-ttu-id="4e2b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e2b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4e2b7-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4e2b7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e2b7-110">Permission type</span></span> | <span data-ttu-id="4e2b7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e2b7-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4e2b7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e2b7-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4e2b7-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="4e2b7-113">Users.Read.All</span></span> |
|<span data-ttu-id="4e2b7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e2b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e2b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-115">Not Supported.</span></span>|
|<span data-ttu-id="4e2b7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e2b7-116">Application</span></span>|<span data-ttu-id="4e2b7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e2b7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e2b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="4e2b7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e2b7-119">Request headers</span></span>
| <span data-ttu-id="4e2b7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4e2b7-120">Name</span></span>      |<span data-ttu-id="4e2b7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e2b7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e2b7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e2b7-122">Authorization</span></span> | <span data-ttu-id="4e2b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e2b7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e2b7-125">Request body</span></span>
<span data-ttu-id="4e2b7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4e2b7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e2b7-127">Response</span></span>
<span data-ttu-id="4e2b7-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Identity](../resources/identity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-128">If successful, this method returns a `200 OK` response code and a collection of [identity](../resources/identity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e2b7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e2b7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e2b7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e2b7-130">Request</span></span>
<span data-ttu-id="4e2b7-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e2b7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e2b7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="4e2b7-133">C#</span><span class="sxs-lookup"><span data-stu-id="4e2b7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e2b7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e2b7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e2b7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e2b7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e2b7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e2b7-136">Response</span></span>
<span data-ttu-id="4e2b7-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-137">The following is an example of the response.</span></span>
><span data-ttu-id="4e2b7-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e2b7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printIdentity)",
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
