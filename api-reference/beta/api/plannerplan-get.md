---
title: Get plannerPlan
description: Recupere as propriedades e os relacionamentos do objeto **plannerplan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6e541b2ab671e22961f4c7c3575c02ee27c10870
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445825"
---
# <a name="get-plannerplan"></a><span data-ttu-id="fde22-103">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fde22-103">Get plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fde22-104">Recupere as propriedades e os relacionamentos do objeto **plannerplan** .</span><span class="sxs-lookup"><span data-stu-id="fde22-104">Retrieve the properties and relationships of **plannerplan** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fde22-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fde22-105">Permissions</span></span>
<span data-ttu-id="fde22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fde22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fde22-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fde22-108">Permission type</span></span>      | <span data-ttu-id="fde22-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fde22-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fde22-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fde22-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fde22-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fde22-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fde22-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fde22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fde22-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fde22-113">Not supported.</span></span>    |
|<span data-ttu-id="fde22-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fde22-114">Application</span></span> | <span data-ttu-id="fde22-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fde22-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fde22-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fde22-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>
```
## <a name="request-headers"></a><span data-ttu-id="fde22-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fde22-117">Request headers</span></span>
| <span data-ttu-id="fde22-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fde22-118">Name</span></span>      |<span data-ttu-id="fde22-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fde22-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fde22-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fde22-120">Authorization</span></span>  | <span data-ttu-id="fde22-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fde22-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fde22-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fde22-123">Request body</span></span>
<span data-ttu-id="fde22-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fde22-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fde22-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="fde22-125">Response</span></span>

<span data-ttu-id="fde22-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fde22-126">If successful, this method returns a `200 OK` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="fde22-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="fde22-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="fde22-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="fde22-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="fde22-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="fde22-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="fde22-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fde22-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fde22-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fde22-131">Request</span></span>
<span data-ttu-id="fde22-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fde22-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fde22-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde22-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fde22-134">C#</span><span class="sxs-lookup"><span data-stu-id="fde22-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fde22-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="fde22-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fde22-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fde22-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fde22-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fde22-137">Response</span></span>
<span data-ttu-id="fde22-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fde22-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
