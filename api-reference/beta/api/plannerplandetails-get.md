---
title: Obter plannerPlanDetails
description: Recupere as propriedades e as relações do **objeto plannerplandetails.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: cdd35ccf974bb8fdf332d54606a13040f6ce66ec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050021"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="3a57b-103">Obter plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="3a57b-103">Get plannerPlanDetails</span></span>

<span data-ttu-id="3a57b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a57b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a57b-105">Recupere as propriedades e as relações do **objeto plannerplandetails.**</span><span class="sxs-lookup"><span data-stu-id="3a57b-105">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a57b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a57b-106">Permissions</span></span>
<span data-ttu-id="3a57b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a57b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a57b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a57b-109">Permission type</span></span>      | <span data-ttu-id="3a57b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a57b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a57b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a57b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3a57b-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a57b-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a57b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a57b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a57b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a57b-114">Not supported.</span></span>    |
|<span data-ttu-id="3a57b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a57b-115">Application</span></span> | <span data-ttu-id="3a57b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a57b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a57b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a57b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="3a57b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a57b-118">Request headers</span></span>
| <span data-ttu-id="3a57b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3a57b-119">Name</span></span>      |<span data-ttu-id="3a57b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a57b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a57b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a57b-121">Authorization</span></span>  | <span data-ttu-id="3a57b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a57b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a57b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a57b-124">Request body</span></span>
<span data-ttu-id="3a57b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a57b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a57b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a57b-126">Response</span></span>

<span data-ttu-id="3a57b-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto plannerPlanDetails](../resources/plannerplandetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a57b-127">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="3a57b-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="3a57b-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="3a57b-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="3a57b-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="3a57b-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="3a57b-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3a57b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a57b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a57b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a57b-132">Request</span></span>
<span data-ttu-id="3a57b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a57b-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a57b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a57b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
```
# <a name="c"></a>[<span data-ttu-id="3a57b-135">C#</span><span class="sxs-lookup"><span data-stu-id="3a57b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a57b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a57b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a57b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a57b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a57b-138">Java</span><span class="sxs-lookup"><span data-stu-id="3a57b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerplandetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3a57b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a57b-139">Response</span></span>
<span data-ttu-id="3a57b-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a57b-140">Here is an example of the response.</span></span> <span data-ttu-id="3a57b-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3a57b-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerPlanDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


