---
title: Listar planos
description: Recupere uma lista de objetos **plannerplan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 77194ba9a656429f62260675bf32dcce4c73baeb
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400623"
---
# <a name="list-plans"></a><span data-ttu-id="4dc2d-103">Listar planos</span><span class="sxs-lookup"><span data-stu-id="4dc2d-103">List plans</span></span>

<span data-ttu-id="4dc2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dc2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4dc2d-105">Recupere uma lista de objetos **plannerplan** .</span><span class="sxs-lookup"><span data-stu-id="4dc2d-105">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4dc2d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4dc2d-106">Permissions</span></span>
<span data-ttu-id="4dc2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dc2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc2d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dc2d-109">Permission type</span></span>      | <span data-ttu-id="4dc2d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4dc2d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dc2d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dc2d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4dc2d-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc2d-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4dc2d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dc2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dc2d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dc2d-114">Not supported.</span></span>    |
|<span data-ttu-id="4dc2d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dc2d-115">Application</span></span> | <span data-ttu-id="4dc2d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dc2d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dc2d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dc2d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4dc2d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4dc2d-118">Optional query parameters</span></span>
<span data-ttu-id="4dc2d-119">Este método requer que o [filtro](/graph/query-parameters) de proprietário seja especificado.</span><span class="sxs-lookup"><span data-stu-id="4dc2d-119">This method requires owner [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4dc2d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc2d-120">Request headers</span></span>
| <span data-ttu-id="4dc2d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4dc2d-121">Name</span></span>      |<span data-ttu-id="4dc2d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dc2d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4dc2d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dc2d-123">Authorization</span></span>  | <span data-ttu-id="4dc2d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dc2d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dc2d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc2d-126">Request body</span></span>
<span data-ttu-id="4dc2d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4dc2d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dc2d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dc2d-128">Response</span></span>

<span data-ttu-id="4dc2d-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dc2d-129">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="4dc2d-130">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="4dc2d-130">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="4dc2d-131">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="4dc2d-131">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="4dc2d-132">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4dc2d-132">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4dc2d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dc2d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4dc2d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc2d-134">Request</span></span>
<span data-ttu-id="4dc2d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dc2d-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4dc2d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4dc2d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/plans
```
# <a name="c"></a>[<span data-ttu-id="4dc2d-137">C#</span><span class="sxs-lookup"><span data-stu-id="4dc2d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4dc2d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4dc2d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4dc2d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4dc2d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4dc2d-140">Java</span><span class="sxs-lookup"><span data-stu-id="4dc2d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4dc2d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dc2d-141">Response</span></span>
<span data-ttu-id="4dc2d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dc2d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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