---
title: Obter plannerProgressTaskBoardTaskFormat
description: Recupere as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 85ec2c4cb40fad58b65f0cfae9fb15c8a0d0c7e6
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725679"
---
# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="3e503-103">Obter plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3e503-103">Get plannerProgressTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e503-104">Recupere as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="3e503-104">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e503-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e503-105">Permissions</span></span>
<span data-ttu-id="3e503-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e503-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e503-108">Permission type</span></span>      | <span data-ttu-id="3e503-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e503-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e503-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e503-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e503-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e503-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e503-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e503-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e503-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e503-113">Not supported.</span></span>    |
|<span data-ttu-id="3e503-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e503-114">Application</span></span> | <span data-ttu-id="3e503-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e503-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e503-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e503-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="3e503-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e503-117">Request headers</span></span>
| <span data-ttu-id="3e503-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3e503-118">Name</span></span>      |<span data-ttu-id="3e503-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e503-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e503-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e503-120">Authorization</span></span>  | <span data-ttu-id="3e503-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e503-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e503-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e503-123">Request body</span></span>
<span data-ttu-id="3e503-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e503-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e503-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e503-125">Response</span></span>

<span data-ttu-id="3e503-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e503-126">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="3e503-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="3e503-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="3e503-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="3e503-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="3e503-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="3e503-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3e503-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e503-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e503-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e503-131">Request</span></span>
<span data-ttu-id="3e503-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e503-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3e503-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e503-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/{id}/progressTaskBoardFormat
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e503-134">C#</span><span class="sxs-lookup"><span data-stu-id="3e503-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e503-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e503-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e503-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3e503-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3e503-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e503-137">Response</span></span>
<span data-ttu-id="3e503-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e503-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "Get plannerProgressTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
