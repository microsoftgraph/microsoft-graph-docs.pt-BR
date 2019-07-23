---
title: Get plannerPlan
description: Recupere as propriedades e os relacionamentos do objeto **plannerplan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: db61db4d793e77d68f4f900e4c921e95e094a12b
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820778"
---
# <a name="get-plannerplan"></a><span data-ttu-id="38b9b-103">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="38b9b-103">Get plannerPlan</span></span>

<span data-ttu-id="38b9b-104">Recupere as propriedades e os relacionamentos de um objeto [plannerplan](../resources/plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="38b9b-104">Retrieve the properties and relationships of a [plannerplan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="38b9b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="38b9b-105">Permissions</span></span>
<span data-ttu-id="38b9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38b9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38b9b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38b9b-108">Permission type</span></span>      | <span data-ttu-id="38b9b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38b9b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38b9b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38b9b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38b9b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38b9b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="38b9b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38b9b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38b9b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38b9b-113">Not supported.</span></span>    |
|<span data-ttu-id="38b9b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38b9b-114">Application</span></span> | <span data-ttu-id="38b9b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38b9b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38b9b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38b9b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}
```
## <a name="request-headers"></a><span data-ttu-id="38b9b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38b9b-117">Request headers</span></span>
| <span data-ttu-id="38b9b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="38b9b-118">Name</span></span>      |<span data-ttu-id="38b9b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="38b9b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38b9b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="38b9b-120">Authorization</span></span>  | <span data-ttu-id="38b9b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38b9b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38b9b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38b9b-123">Request body</span></span>
<span data-ttu-id="38b9b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38b9b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38b9b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="38b9b-125">Response</span></span>

<span data-ttu-id="38b9b-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38b9b-126">If successful, this method returns a `200 OK` response code and a [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="38b9b-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="38b9b-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="38b9b-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="38b9b-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="38b9b-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="38b9b-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="38b9b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38b9b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38b9b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38b9b-131">Request</span></span>
<span data-ttu-id="38b9b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38b9b-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="38b9b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="38b9b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="38b9b-134">C#</span><span class="sxs-lookup"><span data-stu-id="38b9b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38b9b-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="38b9b-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38b9b-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="38b9b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="38b9b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="38b9b-137">Response</span></span>
<span data-ttu-id="38b9b-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38b9b-138">Here is an example of the response.</span></span> 

><span data-ttu-id="38b9b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38b9b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
