---
title: Criar plannerBucket
description: Use essa API para criar um novo **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 45745c40d28e1d9b4826178cc263af9b11bb9bed
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473665"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="4efb3-103">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="4efb3-103">Create plannerBucket</span></span>

<span data-ttu-id="4efb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4efb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4efb3-105">Use essa API para criar um novo **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="4efb3-105">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="4efb3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4efb3-106">Permissions</span></span>
<span data-ttu-id="4efb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4efb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4efb3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4efb3-109">Permission type</span></span>      | <span data-ttu-id="4efb3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4efb3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4efb3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4efb3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4efb3-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4efb3-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4efb3-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4efb3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4efb3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4efb3-114">Not supported.</span></span>    |
|<span data-ttu-id="4efb3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4efb3-115">Application</span></span> | <span data-ttu-id="4efb3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4efb3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4efb3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4efb3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="4efb3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4efb3-118">Request headers</span></span>
| <span data-ttu-id="4efb3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4efb3-119">Name</span></span>       | <span data-ttu-id="4efb3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4efb3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4efb3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4efb3-121">Authorization</span></span>  | <span data-ttu-id="4efb3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4efb3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4efb3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4efb3-124">Request body</span></span>
<span data-ttu-id="4efb3-125">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="4efb3-125">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4efb3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4efb3-126">Response</span></span>

<span data-ttu-id="4efb3-127">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4efb3-127">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="4efb3-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4efb3-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4efb3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4efb3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4efb3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4efb3-132">Request</span></span>
<span data-ttu-id="4efb3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4efb3-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4efb3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4efb3-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4efb3-135">C#</span><span class="sxs-lookup"><span data-stu-id="4efb3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerbucket-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4efb3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4efb3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerbucket-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4efb3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4efb3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerbucket-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4efb3-138">Java</span><span class="sxs-lookup"><span data-stu-id="4efb3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerbucket-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4efb3-139">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="4efb3-139">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4efb3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4efb3-140">Response</span></span>
<span data-ttu-id="4efb3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4efb3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


