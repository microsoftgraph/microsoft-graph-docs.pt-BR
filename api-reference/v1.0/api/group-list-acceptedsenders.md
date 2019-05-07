---
title: Listar acceptedSenders
description: Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c49c4ce96f0842f06c3b9f47783eb84dd9faa77c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614274"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="85daf-103">Listar acceptedSenders</span><span class="sxs-lookup"><span data-stu-id="85daf-103">List acceptedSenders</span></span>
<span data-ttu-id="85daf-104">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.</span><span class="sxs-lookup"><span data-stu-id="85daf-104">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="85daf-p101">Os usuários na lista de remetentes aceitos podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="85daf-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="85daf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="85daf-107">Permissions</span></span>
<span data-ttu-id="85daf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85daf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85daf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85daf-110">Permission type</span></span>      | <span data-ttu-id="85daf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85daf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85daf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85daf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="85daf-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85daf-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="85daf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85daf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85daf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85daf-115">Not supported.</span></span>    |
|<span data-ttu-id="85daf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85daf-116">Application</span></span> | <span data-ttu-id="85daf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85daf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85daf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85daf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85daf-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="85daf-119">Optional query parameters</span></span>
<span data-ttu-id="85daf-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="85daf-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85daf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85daf-121">Request headers</span></span>
| <span data-ttu-id="85daf-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85daf-122">Header</span></span>       | <span data-ttu-id="85daf-123">Valor</span><span class="sxs-lookup"><span data-stu-id="85daf-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85daf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="85daf-124">Authorization</span></span>  | <span data-ttu-id="85daf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85daf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85daf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85daf-127">Request body</span></span>
<span data-ttu-id="85daf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85daf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85daf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="85daf-129">Response</span></span>
<span data-ttu-id="85daf-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85daf-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85daf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85daf-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="85daf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85daf-132">Request</span></span>
<span data-ttu-id="85daf-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85daf-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders
```

#### <a name="response"></a><span data-ttu-id="85daf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="85daf-134">Response</span></span>
<span data-ttu-id="85daf-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85daf-135">The following is an example of the response.</span></span>
><span data-ttu-id="85daf-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85daf-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="85daf-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85daf-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="85daf-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="85daf-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="85daf-139">Basic</span><span class="sxs-lookup"><span data-stu-id="85daf-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_acceptedsenders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85daf-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85daf-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_acceptedsenders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-acceptedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-acceptedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
