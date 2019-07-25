---
title: Listar planos
description: Recupere uma lista de objetos **plannerplan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: eab5de304334c7f17b2ce9dab0453ffa19afc19a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856894"
---
# <a name="list-plans"></a><span data-ttu-id="a6ccc-103">Listar planos</span><span class="sxs-lookup"><span data-stu-id="a6ccc-103">List plans</span></span>

<span data-ttu-id="a6ccc-104">Recupere uma lista de objetos **plannerplan** .</span><span class="sxs-lookup"><span data-stu-id="a6ccc-104">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6ccc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6ccc-105">Permissions</span></span>
<span data-ttu-id="a6ccc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6ccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6ccc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6ccc-108">Permission type</span></span>      | <span data-ttu-id="a6ccc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6ccc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6ccc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6ccc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a6ccc-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6ccc-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6ccc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6ccc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6ccc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6ccc-113">Not supported.</span></span>    |
|<span data-ttu-id="a6ccc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6ccc-114">Application</span></span> | <span data-ttu-id="a6ccc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6ccc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6ccc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6ccc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6ccc-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a6ccc-117">Optional query parameters</span></span>
<span data-ttu-id="a6ccc-118">Este método requer que o [filtro](https://developer.microsoft.com/graph/docs/concepts/query_parameters) de proprietário seja especificado.</span><span class="sxs-lookup"><span data-stu-id="a6ccc-118">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6ccc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ccc-119">Request headers</span></span>
| <span data-ttu-id="a6ccc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a6ccc-120">Name</span></span>      |<span data-ttu-id="a6ccc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6ccc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6ccc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6ccc-122">Authorization</span></span>  | <span data-ttu-id="a6ccc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6ccc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6ccc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ccc-125">Request body</span></span>
<span data-ttu-id="a6ccc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6ccc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6ccc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ccc-127">Response</span></span>

<span data-ttu-id="a6ccc-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6ccc-128">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="a6ccc-129">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="a6ccc-129">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="a6ccc-130">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="a6ccc-130">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="a6ccc-131">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a6ccc-131">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a6ccc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6ccc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6ccc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ccc-133">Request</span></span>
<span data-ttu-id="a6ccc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6ccc-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a6ccc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6ccc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6ccc-136">C#</span><span class="sxs-lookup"><span data-stu-id="a6ccc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6ccc-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a6ccc-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6ccc-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a6ccc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a6ccc-139">Java</span><span class="sxs-lookup"><span data-stu-id="a6ccc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a6ccc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ccc-140">Response</span></span>
<span data-ttu-id="a6ccc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6ccc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 421

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
