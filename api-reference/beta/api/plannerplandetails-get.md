---
title: Obter plannerPlanDetails
description: Recupere as propriedades e os relacionamentos do objeto **plannerplandetails** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: ab21f329a0bc59a420f6669fbb4ba05a9ff91863
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970959"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="ca9e6-103">Obter plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="ca9e6-103">Get plannerPlanDetails</span></span>

<span data-ttu-id="ca9e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca9e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca9e6-105">Recupere as propriedades e os relacionamentos do objeto **plannerplandetails** .</span><span class="sxs-lookup"><span data-stu-id="ca9e6-105">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca9e6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca9e6-106">Permissions</span></span>
<span data-ttu-id="ca9e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca9e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca9e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca9e6-109">Permission type</span></span>      | <span data-ttu-id="ca9e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca9e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca9e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca9e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca9e6-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca9e6-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca9e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca9e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca9e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca9e6-114">Not supported.</span></span>    |
|<span data-ttu-id="ca9e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca9e6-115">Application</span></span> | <span data-ttu-id="ca9e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca9e6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca9e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca9e6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="ca9e6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9e6-118">Request headers</span></span>
| <span data-ttu-id="ca9e6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ca9e6-119">Name</span></span>      |<span data-ttu-id="ca9e6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca9e6-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ca9e6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca9e6-121">Authorization</span></span>  | <span data-ttu-id="ca9e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca9e6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca9e6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9e6-124">Request body</span></span>
<span data-ttu-id="ca9e6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca9e6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca9e6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9e6-126">Response</span></span>

<span data-ttu-id="ca9e6-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerPlanDetails](../resources/plannerplandetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca9e6-127">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="ca9e6-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="ca9e6-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="ca9e6-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="ca9e6-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="ca9e6-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ca9e6-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ca9e6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca9e6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca9e6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9e6-132">Request</span></span>
<span data-ttu-id="ca9e6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca9e6-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca9e6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca9e6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
```
# <a name="c"></a>[<span data-ttu-id="ca9e6-135">C#</span><span class="sxs-lookup"><span data-stu-id="ca9e6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca9e6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca9e6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca9e6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca9e6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca9e6-138">Java</span><span class="sxs-lookup"><span data-stu-id="ca9e6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerplandetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ca9e6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9e6-139">Response</span></span>
<span data-ttu-id="ca9e6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca9e6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


