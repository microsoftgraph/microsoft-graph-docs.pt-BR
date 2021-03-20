---
title: Listar planos
description: Recupere uma lista de objetos **plannerplan.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 4cf4fdbf93cea301e1ddd893d61a0f80664534c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941513"
---
# <a name="list-plans"></a><span data-ttu-id="2e954-103">Listar planos</span><span class="sxs-lookup"><span data-stu-id="2e954-103">List plans</span></span>

<span data-ttu-id="2e954-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e954-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e954-105">Recupere uma lista de objetos **plannerplan.**</span><span class="sxs-lookup"><span data-stu-id="2e954-105">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e954-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e954-106">Permissions</span></span>
<span data-ttu-id="2e954-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e954-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e954-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e954-109">Permission type</span></span>      | <span data-ttu-id="2e954-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e954-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e954-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e954-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e954-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e954-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e954-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e954-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e954-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e954-114">Not supported.</span></span>    |
|<span data-ttu-id="2e954-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e954-115">Application</span></span> | <span data-ttu-id="2e954-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e954-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e954-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e954-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e954-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e954-118">Optional query parameters</span></span>
<span data-ttu-id="2e954-119">Este método exige que [o filtro de](/graph/query-parameters) proprietário seja especificado.</span><span class="sxs-lookup"><span data-stu-id="2e954-119">This method requires owner [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e954-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e954-120">Request headers</span></span>
| <span data-ttu-id="2e954-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2e954-121">Name</span></span>      |<span data-ttu-id="2e954-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e954-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e954-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e954-123">Authorization</span></span>  | <span data-ttu-id="2e954-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e954-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e954-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e954-126">Request body</span></span>
<span data-ttu-id="2e954-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e954-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e954-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e954-128">Response</span></span>

<span data-ttu-id="2e954-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e954-129">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="2e954-130">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="2e954-130">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="2e954-131">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="2e954-131">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="2e954-132">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="2e954-132">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="2e954-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e954-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e954-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e954-134">Request</span></span>
<span data-ttu-id="2e954-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e954-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e954-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e954-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/plans
```
# <a name="c"></a>[<span data-ttu-id="2e954-137">C#</span><span class="sxs-lookup"><span data-stu-id="2e954-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e954-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e954-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e954-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e954-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e954-140">Java</span><span class="sxs-lookup"><span data-stu-id="2e954-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e954-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e954-141">Response</span></span>
<span data-ttu-id="2e954-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e954-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
