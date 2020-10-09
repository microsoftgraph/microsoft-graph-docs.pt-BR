---
title: Obter outlookTaskGroup
description: Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1f0c2cbd766e75f7f440d05a27a0b29d1851e7bc
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400890"
---
# <a name="get-outlooktaskgroup-deprecated"></a><span data-ttu-id="32730-103">Obter outlookTaskGroup (preterido)</span><span class="sxs-lookup"><span data-stu-id="32730-103">Get outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="32730-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32730-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="32730-105">Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="32730-105">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="32730-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="32730-106">Permissions</span></span>
<span data-ttu-id="32730-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32730-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32730-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32730-109">Permission type</span></span>      | <span data-ttu-id="32730-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32730-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32730-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32730-111">Delegated (work or school account)</span></span> | <span data-ttu-id="32730-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="32730-112">Tasks.Read</span></span>    |
|<span data-ttu-id="32730-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32730-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32730-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="32730-114">Tasks.Read</span></span>    |
|<span data-ttu-id="32730-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32730-115">Application</span></span> | <span data-ttu-id="32730-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32730-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32730-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32730-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="32730-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="32730-118">Optional query parameters</span></span>
<span data-ttu-id="32730-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="32730-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32730-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32730-120">Request headers</span></span>
| <span data-ttu-id="32730-121">Nome</span><span class="sxs-lookup"><span data-stu-id="32730-121">Name</span></span>      |<span data-ttu-id="32730-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="32730-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="32730-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32730-123">Authorization</span></span>  | <span data-ttu-id="32730-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32730-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32730-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32730-126">Request body</span></span>
<span data-ttu-id="32730-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32730-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32730-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="32730-128">Response</span></span>

<span data-ttu-id="32730-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32730-129">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32730-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32730-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32730-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32730-131">Request</span></span>
<span data-ttu-id="32730-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32730-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32730-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="32730-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="c"></a>[<span data-ttu-id="32730-134">C#</span><span class="sxs-lookup"><span data-stu-id="32730-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32730-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32730-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32730-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32730-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32730-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="32730-137">Response</span></span>
<span data-ttu-id="32730-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32730-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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