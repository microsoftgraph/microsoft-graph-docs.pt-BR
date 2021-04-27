---
title: Get plannerPlan
description: Recupere as propriedades e as relações do **objeto plannerplan.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 667c188dd186122279e5e13a69ec647f3faa14ed
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037638"
---
# <a name="get-plannerplan"></a><span data-ttu-id="c0554-103">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c0554-103">Get plannerPlan</span></span>

<span data-ttu-id="c0554-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0554-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0554-105">Recupere as propriedades e as relações de um [objeto plannerplan.](../resources/plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="c0554-105">Retrieve the properties and relationships of a [plannerplan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0554-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0554-106">Permissions</span></span>
<span data-ttu-id="c0554-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0554-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0554-109">Permission type</span></span>      | <span data-ttu-id="c0554-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0554-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0554-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0554-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0554-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0554-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c0554-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0554-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0554-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0554-114">Not supported.</span></span>    |
|<span data-ttu-id="c0554-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0554-115">Application</span></span> | <span data-ttu-id="c0554-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0554-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0554-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0554-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}
```
## <a name="request-headers"></a><span data-ttu-id="c0554-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0554-118">Request headers</span></span>
| <span data-ttu-id="c0554-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c0554-119">Name</span></span>      |<span data-ttu-id="c0554-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0554-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0554-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0554-121">Authorization</span></span>  | <span data-ttu-id="c0554-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0554-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0554-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0554-124">Request body</span></span>
<span data-ttu-id="c0554-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0554-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0554-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0554-126">Response</span></span>

<span data-ttu-id="c0554-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0554-127">If successful, this method returns a `200 OK` response code and a [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="c0554-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="c0554-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="c0554-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="c0554-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="c0554-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c0554-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c0554-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0554-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0554-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0554-132">Request</span></span>
<span data-ttu-id="c0554-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0554-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0554-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0554-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/plans/{id}
```
# <a name="c"></a>[<span data-ttu-id="c0554-135">C#</span><span class="sxs-lookup"><span data-stu-id="c0554-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0554-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0554-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0554-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0554-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0554-138">Java</span><span class="sxs-lookup"><span data-stu-id="c0554-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0554-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0554-139">Response</span></span>
<span data-ttu-id="c0554-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0554-140">Here is an example of the response.</span></span> 

><span data-ttu-id="c0554-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c0554-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "url": "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874",
    "containerId": "ebf3b108-5234-4e22-b93d-656d7dae5874",
    "type": "group"
  },
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


