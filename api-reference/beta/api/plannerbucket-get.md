---
title: Obter plannerBucket
description: Recupere as propriedades e os relacionamentos do objeto **plannerBucket** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 25567c85ea43965526860560f8e0a04a6e02c96e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723578"
---
# <a name="get-plannerbucket"></a><span data-ttu-id="e90ca-103">Obter plannerBucket</span><span class="sxs-lookup"><span data-stu-id="e90ca-103">Get plannerBucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e90ca-104">Recupere as propriedades e os relacionamentos do objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="e90ca-104">Retrieve the properties and relationships of **plannerBucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e90ca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e90ca-105">Permissions</span></span>
<span data-ttu-id="e90ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e90ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e90ca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e90ca-108">Permission type</span></span>      | <span data-ttu-id="e90ca-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e90ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e90ca-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e90ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e90ca-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e90ca-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e90ca-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e90ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e90ca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e90ca-113">Not supported.</span></span>    |
|<span data-ttu-id="e90ca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e90ca-114">Application</span></span> | <span data-ttu-id="e90ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e90ca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e90ca-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e90ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e90ca-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e90ca-117">Request headers</span></span>
| <span data-ttu-id="e90ca-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e90ca-118">Name</span></span>      |<span data-ttu-id="e90ca-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e90ca-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e90ca-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e90ca-120">Authorization</span></span>  | <span data-ttu-id="e90ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e90ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e90ca-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e90ca-123">Request body</span></span>
<span data-ttu-id="e90ca-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e90ca-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e90ca-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e90ca-125">Response</span></span>

<span data-ttu-id="e90ca-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e90ca-126">If successful, this method returns a `200 OK` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="e90ca-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="e90ca-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="e90ca-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="e90ca-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="e90ca-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e90ca-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e90ca-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e90ca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e90ca-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e90ca-131">Request</span></span>
<span data-ttu-id="e90ca-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e90ca-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e90ca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e90ca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbucket"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e90ca-134">C#</span><span class="sxs-lookup"><span data-stu-id="e90ca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e90ca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e90ca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e90ca-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e90ca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e90ca-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e90ca-137">Response</span></span>
<span data-ttu-id="e90ca-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e90ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

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
  "description": "Get plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
