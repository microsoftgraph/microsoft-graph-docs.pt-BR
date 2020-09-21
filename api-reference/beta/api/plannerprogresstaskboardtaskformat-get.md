---
title: Obter plannerProgressTaskBoardTaskFormat
description: Recupere as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 7c4d66799351679a306e529ecd52935c6e086f09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966874"
---
# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="60ada-103">Obter plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="60ada-103">Get plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="60ada-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60ada-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60ada-105">Recupere as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="60ada-105">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="60ada-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="60ada-106">Permissions</span></span>
<span data-ttu-id="60ada-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60ada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60ada-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60ada-109">Permission type</span></span>      | <span data-ttu-id="60ada-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60ada-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60ada-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60ada-111">Delegated (work or school account)</span></span> | <span data-ttu-id="60ada-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ada-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60ada-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60ada-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60ada-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60ada-114">Not supported.</span></span>    |
|<span data-ttu-id="60ada-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60ada-115">Application</span></span> | <span data-ttu-id="60ada-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60ada-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60ada-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60ada-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="60ada-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60ada-118">Request headers</span></span>
| <span data-ttu-id="60ada-119">Nome</span><span class="sxs-lookup"><span data-stu-id="60ada-119">Name</span></span>      |<span data-ttu-id="60ada-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="60ada-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60ada-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="60ada-121">Authorization</span></span>  | <span data-ttu-id="60ada-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60ada-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60ada-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60ada-124">Request body</span></span>
<span data-ttu-id="60ada-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60ada-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60ada-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="60ada-126">Response</span></span>

<span data-ttu-id="60ada-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60ada-127">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="60ada-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="60ada-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="60ada-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="60ada-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="60ada-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="60ada-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="60ada-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60ada-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60ada-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60ada-132">Request</span></span>
<span data-ttu-id="60ada-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60ada-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60ada-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="60ada-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/{id}/progressTaskBoardFormat
```
# <a name="c"></a>[<span data-ttu-id="60ada-135">C#</span><span class="sxs-lookup"><span data-stu-id="60ada-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60ada-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60ada-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60ada-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60ada-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="60ada-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="60ada-138">Response</span></span>
<span data-ttu-id="60ada-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60ada-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


