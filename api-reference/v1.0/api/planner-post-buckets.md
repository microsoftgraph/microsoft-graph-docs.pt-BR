---
title: Criar plannerBucket
description: Use essa API para criar um novo **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9a72d4d330b83b1e11af66d67f7b1f44208d0c2b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274225"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="9a919-103">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9a919-103">Create plannerBucket</span></span>

<span data-ttu-id="9a919-104">Use essa API para criar um novo **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="9a919-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a919-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a919-105">Permissions</span></span>
<span data-ttu-id="9a919-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a919-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a919-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a919-108">Permission type</span></span>      | <span data-ttu-id="9a919-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a919-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a919-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a919-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a919-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a919-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a919-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a919-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a919-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a919-113">Not supported.</span></span>    |
|<span data-ttu-id="9a919-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a919-114">Application</span></span> | <span data-ttu-id="9a919-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a919-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a919-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a919-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="9a919-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a919-117">Request headers</span></span>
| <span data-ttu-id="9a919-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9a919-118">Name</span></span>       | <span data-ttu-id="9a919-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a919-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a919-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a919-120">Authorization</span></span>  | <span data-ttu-id="9a919-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a919-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a919-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a919-123">Request body</span></span>
<span data-ttu-id="9a919-124">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="9a919-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9a919-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a919-125">Response</span></span>

<span data-ttu-id="9a919-126">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a919-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="9a919-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="9a919-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9a919-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a919-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a919-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a919-131">Request</span></span>
<span data-ttu-id="9a919-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a919-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
<span data-ttu-id="9a919-133">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="9a919-133">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9a919-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a919-134">Response</span></span>
<span data-ttu-id="9a919-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a919-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9a919-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9a919-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9a919-139">C#</span><span class="sxs-lookup"><span data-stu-id="9a919-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_plannerbucket_from_planner-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a919-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a919-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_plannerbucket_from_planner-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9a919-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9a919-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_plannerbucket_from_planner-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/planner-post-buckets.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/planner-post-buckets.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/planner-post-buckets.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
