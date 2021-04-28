---
title: Listar planos
description: Recupere uma lista de objetos **plannerplan.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 7a5f4d7fb86a87c2fd2ec865a8e4e95ead6205c1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035229"
---
# <a name="list-plans"></a><span data-ttu-id="22a17-103">Listar planos</span><span class="sxs-lookup"><span data-stu-id="22a17-103">List plans</span></span>

<span data-ttu-id="22a17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a17-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22a17-105">Recupere uma lista de objetos **plannerplan.**</span><span class="sxs-lookup"><span data-stu-id="22a17-105">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="22a17-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22a17-106">Permissions</span></span>
<span data-ttu-id="22a17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a17-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22a17-109">Permission type</span></span>      | <span data-ttu-id="22a17-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22a17-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22a17-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22a17-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22a17-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a17-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="22a17-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22a17-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22a17-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22a17-114">Not supported.</span></span>    |
|<span data-ttu-id="22a17-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22a17-115">Application</span></span> | <span data-ttu-id="22a17-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22a17-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22a17-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22a17-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="22a17-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22a17-118">Optional query parameters</span></span>
<span data-ttu-id="22a17-119">Este método exige que [o filtro de](/graph/query-parameters) proprietário seja especificado.</span><span class="sxs-lookup"><span data-stu-id="22a17-119">This method requires owner [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22a17-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22a17-120">Request headers</span></span>
| <span data-ttu-id="22a17-121">Nome</span><span class="sxs-lookup"><span data-stu-id="22a17-121">Name</span></span>      |<span data-ttu-id="22a17-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a17-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22a17-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22a17-123">Authorization</span></span>  | <span data-ttu-id="22a17-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22a17-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22a17-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22a17-126">Request body</span></span>
<span data-ttu-id="22a17-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22a17-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22a17-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a17-128">Response</span></span>

<span data-ttu-id="22a17-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22a17-129">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="22a17-130">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="22a17-130">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="22a17-131">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="22a17-131">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="22a17-132">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="22a17-132">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="22a17-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22a17-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22a17-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22a17-134">Request</span></span>
<span data-ttu-id="22a17-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22a17-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22a17-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="22a17-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/plans
```
# <a name="c"></a>[<span data-ttu-id="22a17-137">C#</span><span class="sxs-lookup"><span data-stu-id="22a17-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22a17-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22a17-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22a17-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22a17-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22a17-140">Java</span><span class="sxs-lookup"><span data-stu-id="22a17-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="22a17-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a17-141">Response</span></span>
<span data-ttu-id="22a17-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22a17-142">Here is an example of the response.</span></span> <span data-ttu-id="22a17-143">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="22a17-143">Note: The response object shown here might be shortened for readability.</span></span>
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
