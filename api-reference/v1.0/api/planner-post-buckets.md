---
title: Criar plannerBucket
description: Use essa API para criar um novo **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4ab94c24903ec761b1f4a0098b507c1f97395c57
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856881"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="910bb-103">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="910bb-103">Create plannerBucket</span></span>

<span data-ttu-id="910bb-104">Use essa API para criar um novo **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="910bb-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="910bb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="910bb-105">Permissions</span></span>
<span data-ttu-id="910bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="910bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="910bb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="910bb-108">Permission type</span></span>      | <span data-ttu-id="910bb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="910bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="910bb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="910bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="910bb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="910bb-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="910bb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="910bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="910bb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="910bb-113">Not supported.</span></span>    |
|<span data-ttu-id="910bb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="910bb-114">Application</span></span> | <span data-ttu-id="910bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="910bb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="910bb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="910bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="910bb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="910bb-117">Request headers</span></span>
| <span data-ttu-id="910bb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="910bb-118">Name</span></span>       | <span data-ttu-id="910bb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="910bb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="910bb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="910bb-120">Authorization</span></span>  | <span data-ttu-id="910bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="910bb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="910bb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="910bb-123">Request body</span></span>
<span data-ttu-id="910bb-124">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="910bb-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="910bb-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="910bb-125">Response</span></span>

<span data-ttu-id="910bb-126">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="910bb-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="910bb-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="910bb-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="910bb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="910bb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="910bb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="910bb-131">Request</span></span>
<span data-ttu-id="910bb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="910bb-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="910bb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="910bb-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="910bb-134">C#</span><span class="sxs-lookup"><span data-stu-id="910bb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerbucket-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="910bb-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="910bb-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerbucket-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="910bb-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="910bb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerbucket-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="910bb-137">Java</span><span class="sxs-lookup"><span data-stu-id="910bb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerbucket-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="910bb-138">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="910bb-138">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="910bb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="910bb-139">Response</span></span>
<span data-ttu-id="910bb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="910bb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
