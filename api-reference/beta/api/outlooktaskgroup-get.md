---
title: Obter outlookTaskGroup
description: Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8d3d5b164d3bdcfee98f9f664afd187b91d9f016
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456115"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="93b0e-103">Obter outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="93b0e-103">Get outlookTaskGroup</span></span>

<span data-ttu-id="93b0e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="93b0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93b0e-105">Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="93b0e-105">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="93b0e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93b0e-106">Permissions</span></span>
<span data-ttu-id="93b0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93b0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93b0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93b0e-109">Permission type</span></span>      | <span data-ttu-id="93b0e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93b0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93b0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93b0e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93b0e-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="93b0e-112">Tasks.Read</span></span>    |
|<span data-ttu-id="93b0e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93b0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93b0e-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="93b0e-114">Tasks.Read</span></span>    |
|<span data-ttu-id="93b0e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93b0e-115">Application</span></span> | <span data-ttu-id="93b0e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93b0e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93b0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93b0e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93b0e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="93b0e-118">Optional query parameters</span></span>
<span data-ttu-id="93b0e-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="93b0e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93b0e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93b0e-120">Request headers</span></span>
| <span data-ttu-id="93b0e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="93b0e-121">Name</span></span>      |<span data-ttu-id="93b0e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="93b0e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93b0e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93b0e-123">Authorization</span></span>  | <span data-ttu-id="93b0e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93b0e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93b0e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93b0e-126">Request body</span></span>
<span data-ttu-id="93b0e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93b0e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93b0e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="93b0e-128">Response</span></span>

<span data-ttu-id="93b0e-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93b0e-129">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93b0e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93b0e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93b0e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93b0e-131">Request</span></span>
<span data-ttu-id="93b0e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93b0e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93b0e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="93b0e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="c"></a>[<span data-ttu-id="93b0e-134">C#</span><span class="sxs-lookup"><span data-stu-id="93b0e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93b0e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93b0e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93b0e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93b0e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="93b0e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="93b0e-137">Response</span></span>
<span data-ttu-id="93b0e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93b0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
