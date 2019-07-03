---
title: Obter plannerTask
description: Recupere as propriedades e os relacionamentos do objeto **plannertask** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 762ced46fa17a7fe33fec2ac5e92480069ba74ca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445783"
---
# <a name="get-plannertask"></a><span data-ttu-id="113ea-103">Obter plannerTask</span><span class="sxs-lookup"><span data-stu-id="113ea-103">Get plannerTask</span></span>

<span data-ttu-id="113ea-104">Recupere as propriedades e os relacionamentos do objeto **plannertask** .</span><span class="sxs-lookup"><span data-stu-id="113ea-104">Retrieve the properties and relationships of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="113ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="113ea-105">Permissions</span></span>
<span data-ttu-id="113ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="113ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="113ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="113ea-108">Permission type</span></span>      | <span data-ttu-id="113ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="113ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="113ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="113ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="113ea-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="113ea-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="113ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="113ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="113ea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="113ea-113">Not supported.</span></span>    |
|<span data-ttu-id="113ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="113ea-114">Application</span></span> | <span data-ttu-id="113ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="113ea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="113ea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="113ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="113ea-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="113ea-117">Request headers</span></span>
| <span data-ttu-id="113ea-118">Nome</span><span class="sxs-lookup"><span data-stu-id="113ea-118">Name</span></span>      |<span data-ttu-id="113ea-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="113ea-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="113ea-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="113ea-120">Authorization</span></span>  | <span data-ttu-id="113ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="113ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="113ea-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="113ea-123">Request body</span></span>
<span data-ttu-id="113ea-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="113ea-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="113ea-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="113ea-125">Response</span></span>

<span data-ttu-id="113ea-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="113ea-126">If successful, this method returns a `200 OK` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="113ea-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="113ea-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="113ea-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="113ea-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="113ea-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="113ea-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="113ea-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="113ea-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="113ea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="113ea-131">Request</span></span>
<span data-ttu-id="113ea-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="113ea-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="113ea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="113ea-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="113ea-134">C#</span><span class="sxs-lookup"><span data-stu-id="113ea-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="113ea-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="113ea-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="113ea-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="113ea-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannertask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="113ea-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="113ea-137">Response</span></span>
<span data-ttu-id="113ea-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="113ea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 707

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
  "title": "title-value",
  "orderHint": "9223370609546166567W",
  "assigneePriority": "90057581\"",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
