---
title: Listar allowedGroups
description: Recupere uma lista de grupos aos quais o acesso foi concedido para enviar trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 22943f9ffaaee83922d9ecaca41b6307c56ea97e
ms.sourcegitcommit: d2536f56e3a424219660bc0495ec8632932b4fb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2020
ms.locfileid: "43812495"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="ac6bd-103">Listar allowedGroups</span><span class="sxs-lookup"><span data-stu-id="ac6bd-103">List allowedGroups</span></span>

<span data-ttu-id="ac6bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac6bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac6bd-105">Recupere uma lista de grupos aos quais o acesso foi concedido para enviar trabalhos de impressão à [impressora](../resources/printer.md)associada.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac6bd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac6bd-106">Permissions</span></span>
<span data-ttu-id="ac6bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac6bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ac6bd-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="ac6bd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac6bd-110">Permission type</span></span> | <span data-ttu-id="ac6bd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac6bd-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ac6bd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac6bd-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ac6bd-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="ac6bd-113">Users.Read.All</span></span> |
|<span data-ttu-id="ac6bd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac6bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac6bd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-115">Not Supported.</span></span>|
|<span data-ttu-id="ac6bd-116">Application</span><span class="sxs-lookup"><span data-stu-id="ac6bd-116">Application</span></span>|<span data-ttu-id="ac6bd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac6bd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac6bd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac6bd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ac6bd-119">Optional query parameters</span></span>
<span data-ttu-id="ac6bd-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ac6bd-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ac6bd-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac6bd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac6bd-122">Request headers</span></span>
| <span data-ttu-id="ac6bd-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ac6bd-123">Name</span></span>      |<span data-ttu-id="ac6bd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac6bd-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac6bd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac6bd-125">Authorization</span></span> | <span data-ttu-id="ac6bd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac6bd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac6bd-128">Request body</span></span>
<span data-ttu-id="ac6bd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ac6bd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac6bd-130">Response</span></span>
<span data-ttu-id="ac6bd-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Identity](../resources/identity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-131">If successful, this method returns a `200 OK` response code and a collection of [identity](../resources/identity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ac6bd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac6bd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac6bd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac6bd-133">Request</span></span>
<span data-ttu-id="ac6bd-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac6bd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac6bd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="ac6bd-136">C#</span><span class="sxs-lookup"><span data-stu-id="ac6bd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac6bd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac6bd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac6bd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac6bd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ac6bd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac6bd-139">Response</span></span>
<span data-ttu-id="ac6bd-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-140">The following is an example of the response.</span></span>
><span data-ttu-id="ac6bd-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac6bd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
