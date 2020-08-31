---
title: Obter outlookTaskGroup
description: Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7c164e94898b4e5ea6836c5b9ae0787a516cc5bf
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311603"
---
# <a name="get-outlooktaskgroup-deprecated"></a><span data-ttu-id="84120-103">Obter outlookTaskGroup (preterido)</span><span class="sxs-lookup"><span data-stu-id="84120-103">Get outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="84120-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84120-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="84120-105">Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="84120-105">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="84120-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="84120-106">Permissions</span></span>
<span data-ttu-id="84120-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84120-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84120-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84120-109">Permission type</span></span>      | <span data-ttu-id="84120-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84120-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84120-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84120-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84120-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="84120-112">Tasks.Read</span></span>    |
|<span data-ttu-id="84120-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84120-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84120-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="84120-114">Tasks.Read</span></span>    |
|<span data-ttu-id="84120-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84120-115">Application</span></span> | <span data-ttu-id="84120-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84120-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84120-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84120-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84120-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="84120-118">Optional query parameters</span></span>
<span data-ttu-id="84120-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="84120-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84120-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84120-120">Request headers</span></span>
| <span data-ttu-id="84120-121">Nome</span><span class="sxs-lookup"><span data-stu-id="84120-121">Name</span></span>      |<span data-ttu-id="84120-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="84120-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84120-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84120-123">Authorization</span></span>  | <span data-ttu-id="84120-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84120-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84120-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84120-126">Request body</span></span>
<span data-ttu-id="84120-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84120-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84120-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="84120-128">Response</span></span>

<span data-ttu-id="84120-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84120-129">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84120-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84120-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84120-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84120-131">Request</span></span>
<span data-ttu-id="84120-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84120-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84120-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="84120-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="c"></a>[<span data-ttu-id="84120-134">C#</span><span class="sxs-lookup"><span data-stu-id="84120-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84120-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84120-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84120-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84120-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84120-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="84120-137">Response</span></span>
<span data-ttu-id="84120-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84120-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
    "id": "AAMkADIyAAAhrbe-AAA=",
    "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
    "isDefaultGroup": false,
    "name": "Leisure Tasks",
    "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
