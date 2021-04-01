---
title: Get plannerPlan
description: Recupere as propriedades e as relações do **objeto plannerplan.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 570be9cfe55b6c41ed0e2bf44a4566e41da92ea8
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473868"
---
# <a name="get-plannerplan"></a><span data-ttu-id="497ff-103">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="497ff-103">Get plannerPlan</span></span>

<span data-ttu-id="497ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="497ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="497ff-105">Recupere as propriedades e as relações de um [objeto plannerplan.](../resources/plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="497ff-105">Retrieve the properties and relationships of a [plannerplan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="497ff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="497ff-106">Permissions</span></span>
<span data-ttu-id="497ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="497ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="497ff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="497ff-109">Permission type</span></span>      | <span data-ttu-id="497ff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="497ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="497ff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="497ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="497ff-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497ff-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="497ff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="497ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="497ff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="497ff-114">Not supported.</span></span>    |
|<span data-ttu-id="497ff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="497ff-115">Application</span></span> | <span data-ttu-id="497ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="497ff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="497ff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="497ff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}
```
## <a name="request-headers"></a><span data-ttu-id="497ff-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="497ff-118">Request headers</span></span>
| <span data-ttu-id="497ff-119">Nome</span><span class="sxs-lookup"><span data-stu-id="497ff-119">Name</span></span>      |<span data-ttu-id="497ff-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="497ff-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="497ff-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="497ff-121">Authorization</span></span>  | <span data-ttu-id="497ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="497ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="497ff-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="497ff-124">Request body</span></span>
<span data-ttu-id="497ff-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="497ff-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="497ff-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="497ff-126">Response</span></span>

<span data-ttu-id="497ff-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="497ff-127">If successful, this method returns a `200 OK` response code and a [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="497ff-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="497ff-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="497ff-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="497ff-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="497ff-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="497ff-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="497ff-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="497ff-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="497ff-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="497ff-132">Request</span></span>
<span data-ttu-id="497ff-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="497ff-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="497ff-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="497ff-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
```
# <a name="c"></a>[<span data-ttu-id="497ff-135">C#</span><span class="sxs-lookup"><span data-stu-id="497ff-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="497ff-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="497ff-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="497ff-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="497ff-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="497ff-138">Java</span><span class="sxs-lookup"><span data-stu-id="497ff-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="497ff-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="497ff-139">Response</span></span>
<span data-ttu-id="497ff-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="497ff-140">Here is an example of the response.</span></span> 

><span data-ttu-id="497ff-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="497ff-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

