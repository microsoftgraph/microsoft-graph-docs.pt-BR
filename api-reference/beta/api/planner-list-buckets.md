---
title: Listar buckets
description: Recupere uma lista de objetos **plannerbucket** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 950faaa372de5567f9ee0bb451975f005c976c11
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315217"
---
# <a name="list-buckets"></a><span data-ttu-id="bf9af-103">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="bf9af-103">List buckets</span></span>

<span data-ttu-id="bf9af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf9af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf9af-105">Recupere uma lista de objetos **plannerbucket** .</span><span class="sxs-lookup"><span data-stu-id="bf9af-105">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf9af-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf9af-106">Permissions</span></span>
<span data-ttu-id="bf9af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf9af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf9af-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf9af-109">Permission type</span></span>      | <span data-ttu-id="bf9af-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf9af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf9af-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf9af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf9af-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9af-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bf9af-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf9af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf9af-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf9af-114">Not supported.</span></span>    |
|<span data-ttu-id="bf9af-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf9af-115">Application</span></span> | <span data-ttu-id="bf9af-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf9af-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf9af-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf9af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bf9af-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bf9af-118">Optional query parameters</span></span>
<span data-ttu-id="bf9af-119">Este método requer que o [filtro](/graph/query-parameters) de PlanID seja especificado.</span><span class="sxs-lookup"><span data-stu-id="bf9af-119">This method requires planId [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf9af-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf9af-120">Request headers</span></span>
| <span data-ttu-id="bf9af-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bf9af-121">Name</span></span>      |<span data-ttu-id="bf9af-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf9af-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bf9af-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf9af-123">Authorization</span></span>  | <span data-ttu-id="bf9af-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf9af-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf9af-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf9af-126">Request body</span></span>
<span data-ttu-id="bf9af-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bf9af-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf9af-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf9af-128">Response</span></span>

<span data-ttu-id="bf9af-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf9af-129">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="bf9af-130">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="bf9af-130">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="bf9af-131">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="bf9af-131">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="bf9af-132">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="bf9af-132">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="bf9af-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf9af-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf9af-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf9af-134">Request</span></span>
<span data-ttu-id="bf9af-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf9af-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf9af-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf9af-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/buckets
```
# <a name="c"></a>[<span data-ttu-id="bf9af-137">C#</span><span class="sxs-lookup"><span data-stu-id="bf9af-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf9af-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf9af-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf9af-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf9af-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bf9af-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf9af-140">Response</span></span>
<span data-ttu-id="bf9af-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf9af-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->