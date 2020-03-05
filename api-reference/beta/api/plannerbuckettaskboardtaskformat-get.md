---
title: Obter plannerBucketTaskBoardTaskFormat
description: Recupere as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 93d4b465757dc2effc2a2191f9b5fcedf9ae7efe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455715"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="ad291-103">Obter plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ad291-103">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="ad291-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ad291-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad291-105">Recupere as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="ad291-105">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad291-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad291-106">Permissions</span></span>
<span data-ttu-id="ad291-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad291-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad291-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad291-109">Permission type</span></span>      | <span data-ttu-id="ad291-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad291-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad291-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad291-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad291-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad291-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad291-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad291-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad291-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad291-114">Not supported.</span></span>    |
|<span data-ttu-id="ad291-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad291-115">Application</span></span> | <span data-ttu-id="ad291-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad291-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad291-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad291-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="ad291-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad291-118">Request headers</span></span>
| <span data-ttu-id="ad291-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ad291-119">Name</span></span>      |<span data-ttu-id="ad291-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad291-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad291-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad291-121">Authorization</span></span>  | <span data-ttu-id="ad291-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad291-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad291-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad291-124">Request body</span></span>
<span data-ttu-id="ad291-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad291-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad291-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad291-126">Response</span></span>

<span data-ttu-id="ad291-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad291-127">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="ad291-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="ad291-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="ad291-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="ad291-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="ad291-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ad291-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ad291-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad291-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad291-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad291-132">Request</span></span>
<span data-ttu-id="ad291-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad291-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad291-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad291-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
# <a name="c"></a>[<span data-ttu-id="ad291-135">C#</span><span class="sxs-lookup"><span data-stu-id="ad291-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad291-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad291-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad291-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad291-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ad291-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad291-138">Response</span></span>
<span data-ttu-id="ad291-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad291-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
