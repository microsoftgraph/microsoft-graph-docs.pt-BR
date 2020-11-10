---
title: Obter plannerBucketTaskBoardTaskFormat
description: Recupere as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 86f4b7f908159957258ad9485fdd6f3e964404a2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978281"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="370a3-103">Obter plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="370a3-103">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="370a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="370a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="370a3-105">Recupere as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="370a3-105">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="370a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="370a3-106">Permissions</span></span>
<span data-ttu-id="370a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="370a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="370a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="370a3-109">Permission type</span></span>      | <span data-ttu-id="370a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="370a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="370a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="370a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="370a3-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="370a3-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="370a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="370a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="370a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="370a3-114">Not supported.</span></span>    |
|<span data-ttu-id="370a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="370a3-115">Application</span></span> | <span data-ttu-id="370a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="370a3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="370a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="370a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="370a3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="370a3-118">Request headers</span></span>
| <span data-ttu-id="370a3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="370a3-119">Name</span></span>      |<span data-ttu-id="370a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="370a3-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="370a3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="370a3-121">Authorization</span></span>  | <span data-ttu-id="370a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="370a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="370a3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="370a3-124">Request body</span></span>
<span data-ttu-id="370a3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="370a3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="370a3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="370a3-126">Response</span></span>

<span data-ttu-id="370a3-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="370a3-127">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="370a3-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="370a3-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="370a3-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="370a3-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="370a3-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="370a3-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="370a3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="370a3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="370a3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="370a3-132">Request</span></span>
<span data-ttu-id="370a3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="370a3-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="370a3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="370a3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
# <a name="c"></a>[<span data-ttu-id="370a3-135">C#</span><span class="sxs-lookup"><span data-stu-id="370a3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="370a3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="370a3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="370a3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="370a3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="370a3-138">Java</span><span class="sxs-lookup"><span data-stu-id="370a3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerbuckettaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="370a3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="370a3-139">Response</span></span>
<span data-ttu-id="370a3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="370a3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


