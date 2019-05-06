---
title: Listar buckets
description: Recupere uma lista de objetos **plannerbucket** contidos em um objeto plannerPlan.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 3a1d079e4fb8e5f50c4bf9e408bdf343bd41cb8f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594909"
---
# <a name="list-buckets"></a><span data-ttu-id="f2560-103">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="f2560-103">List buckets</span></span>

<span data-ttu-id="f2560-104">Recupere uma lista de objetos **plannerbucket** contidos em um objeto [plannerPlan](../resources/plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="f2560-104">Retrieve a list of **plannerbucket** objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2560-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2560-105">Permissions</span></span>
<span data-ttu-id="f2560-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2560-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2560-108">Permission type</span></span>      | <span data-ttu-id="f2560-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2560-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2560-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2560-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f2560-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2560-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2560-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2560-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2560-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2560-113">Not supported.</span></span>    |
|<span data-ttu-id="f2560-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2560-114">Application</span></span> | <span data-ttu-id="f2560-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2560-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2560-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2560-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="f2560-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2560-117">Request headers</span></span>
| <span data-ttu-id="f2560-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f2560-118">Name</span></span>      |<span data-ttu-id="f2560-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2560-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2560-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2560-120">Authorization</span></span>  | <span data-ttu-id="f2560-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2560-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2560-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2560-123">Request body</span></span>
<span data-ttu-id="f2560-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2560-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2560-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2560-125">Response</span></span>

<span data-ttu-id="f2560-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2560-126">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="f2560-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="f2560-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="f2560-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="f2560-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="f2560-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f2560-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="f2560-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2560-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2560-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2560-131">Request</span></span>
<span data-ttu-id="f2560-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2560-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/buckets
```
##### <a name="response"></a><span data-ttu-id="f2560-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2560-133">Response</span></span>
<span data-ttu-id="f2560-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2560-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f2560-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f2560-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f2560-138">Basic</span><span class="sxs-lookup"><span data-stu-id="f2560-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_buckets-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2560-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2560-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_buckets-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerplan-list-buckets.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerplan-list-buckets.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
