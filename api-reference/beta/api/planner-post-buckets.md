---
title: Criar plannerBucket
description: Use essa API para criar um novo **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 2ab7899ffac413aa885c5d3c8e89399e95edbfb0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055355"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="6b066-103">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="6b066-103">Create plannerBucket</span></span>

<span data-ttu-id="6b066-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b066-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b066-105">Use essa API para criar um novo **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="6b066-105">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b066-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b066-106">Permissions</span></span>
<span data-ttu-id="6b066-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b066-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b066-109">Permission type</span></span>      | <span data-ttu-id="6b066-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b066-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b066-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b066-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b066-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b066-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b066-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b066-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b066-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b066-114">Not supported.</span></span>    |
|<span data-ttu-id="6b066-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b066-115">Application</span></span> | <span data-ttu-id="6b066-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b066-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b066-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b066-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="6b066-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b066-118">Request headers</span></span>
| <span data-ttu-id="6b066-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b066-119">Name</span></span>       | <span data-ttu-id="6b066-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b066-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6b066-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b066-121">Authorization</span></span>  | <span data-ttu-id="6b066-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b066-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b066-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b066-124">Request body</span></span>
<span data-ttu-id="6b066-125">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="6b066-125">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6b066-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b066-126">Response</span></span>

<span data-ttu-id="6b066-127">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b066-127">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="6b066-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="6b066-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6b066-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b066-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b066-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b066-132">Request</span></span>
<span data-ttu-id="6b066-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b066-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b066-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b066-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
# <a name="c"></a>[<span data-ttu-id="6b066-135">C#</span><span class="sxs-lookup"><span data-stu-id="6b066-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerbucket-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b066-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b066-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerbucket-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b066-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b066-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerbucket-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b066-138">Java</span><span class="sxs-lookup"><span data-stu-id="6b066-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerbucket-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="6b066-139">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="6b066-139">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6b066-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b066-140">Response</span></span>
<span data-ttu-id="6b066-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b066-141">Here is an example of the response.</span></span> <span data-ttu-id="6b066-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6b066-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


