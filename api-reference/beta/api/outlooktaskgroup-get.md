---
title: Obter outlookTaskGroup
description: Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7e8896515f46a05443cad33d5e39ec233018727c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349758"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="70f56-103">Obter outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="70f56-103">Get outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70f56-104">Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="70f56-104">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="70f56-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="70f56-105">Permissions</span></span>
<span data-ttu-id="70f56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70f56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70f56-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70f56-108">Permission type</span></span>      | <span data-ttu-id="70f56-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70f56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70f56-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70f56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70f56-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="70f56-111">Tasks.Read</span></span>    |
|<span data-ttu-id="70f56-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70f56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70f56-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="70f56-113">Tasks.Read</span></span>    |
|<span data-ttu-id="70f56-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70f56-114">Application</span></span> | <span data-ttu-id="70f56-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70f56-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70f56-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70f56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70f56-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="70f56-117">Optional query parameters</span></span>
<span data-ttu-id="70f56-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="70f56-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70f56-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70f56-119">Request headers</span></span>
| <span data-ttu-id="70f56-120">Nome</span><span class="sxs-lookup"><span data-stu-id="70f56-120">Name</span></span>      |<span data-ttu-id="70f56-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="70f56-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70f56-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="70f56-122">Authorization</span></span>  | <span data-ttu-id="70f56-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70f56-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70f56-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70f56-125">Request body</span></span>
<span data-ttu-id="70f56-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70f56-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70f56-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="70f56-127">Response</span></span>

<span data-ttu-id="70f56-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70f56-128">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70f56-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70f56-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70f56-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70f56-130">Request</span></span>
<span data-ttu-id="70f56-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70f56-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="70f56-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="70f56-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70f56-133">C#</span><span class="sxs-lookup"><span data-stu-id="70f56-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70f56-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70f56-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70f56-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="70f56-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="70f56-136">Java</span><span class="sxs-lookup"><span data-stu-id="70f56-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="70f56-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="70f56-137">Response</span></span>
<span data-ttu-id="70f56-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70f56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
