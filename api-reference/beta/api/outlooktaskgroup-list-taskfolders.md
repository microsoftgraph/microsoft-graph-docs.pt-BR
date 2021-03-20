---
title: Listar taskFolders
description: Obter pastas de tarefas do Outlook em um outlookTaskGroup específico.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bc83f3d5c17f5d2f40b2d13440633b088674577d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953258"
---
# <a name="list-taskfolders-deprecated"></a><span data-ttu-id="0105e-103">Listar taskFolders (preterido)</span><span class="sxs-lookup"><span data-stu-id="0105e-103">List taskFolders (deprecated)</span></span>

<span data-ttu-id="0105e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0105e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="0105e-105">Obter pastas de tarefas do Outlook em um [outlookTaskGroup específico.](../resources/outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0105e-105">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0105e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0105e-106">Permissions</span></span>
<span data-ttu-id="0105e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0105e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0105e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0105e-109">Permission type</span></span>      | <span data-ttu-id="0105e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0105e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0105e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0105e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0105e-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0105e-112">Tasks.Read</span></span>    |
|<span data-ttu-id="0105e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0105e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0105e-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0105e-114">Tasks.Read</span></span>    |
|<span data-ttu-id="0105e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0105e-115">Application</span></span> | <span data-ttu-id="0105e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0105e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0105e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0105e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0105e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0105e-118">Optional query parameters</span></span>
<span data-ttu-id="0105e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0105e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0105e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0105e-120">Request headers</span></span>
| <span data-ttu-id="0105e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0105e-121">Name</span></span>      |<span data-ttu-id="0105e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0105e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0105e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0105e-123">Authorization</span></span>  | <span data-ttu-id="0105e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0105e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0105e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0105e-126">Request body</span></span>
<span data-ttu-id="0105e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0105e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0105e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0105e-128">Response</span></span>

<span data-ttu-id="0105e-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0105e-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0105e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0105e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0105e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0105e-131">Request</span></span>
<span data-ttu-id="0105e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0105e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0105e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0105e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders
```
# <a name="c"></a>[<span data-ttu-id="0105e-134">C#</span><span class="sxs-lookup"><span data-stu-id="0105e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0105e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0105e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0105e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0105e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0105e-137">Java</span><span class="sxs-lookup"><span data-stu-id="0105e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskfolders-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0105e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0105e-138">Response</span></span>
<span data-ttu-id="0105e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0105e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "value": [
    {
      "id": "AAMkADIyAAAhrbPXAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
      "isDefaultFolder": false,
      "name": "Cooking",
      "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
