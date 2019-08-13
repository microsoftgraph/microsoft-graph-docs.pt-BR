---
title: Listar taskFolders
description: Obter pastas de tarefas do Outlook em um outlookTaskGroup específico.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1c61a5c07f23932789e0e9d28b8d176001c31f64
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349695"
---
# <a name="list-taskfolders"></a><span data-ttu-id="da058-103">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="da058-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da058-104">Obter pastas de tarefas do Outlook em um [outlookTaskGroup](../resources/outlooktaskgroup.md)específico.</span><span class="sxs-lookup"><span data-stu-id="da058-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="da058-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="da058-105">Permissions</span></span>
<span data-ttu-id="da058-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da058-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da058-108">Permission type</span></span>      | <span data-ttu-id="da058-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da058-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da058-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da058-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da058-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="da058-111">Tasks.Read</span></span>    |
|<span data-ttu-id="da058-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da058-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da058-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="da058-113">Tasks.Read</span></span>    |
|<span data-ttu-id="da058-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da058-114">Application</span></span> | <span data-ttu-id="da058-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da058-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da058-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da058-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="da058-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da058-117">Optional query parameters</span></span>
<span data-ttu-id="da058-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da058-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da058-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da058-119">Request headers</span></span>
| <span data-ttu-id="da058-120">Nome</span><span class="sxs-lookup"><span data-stu-id="da058-120">Name</span></span>      |<span data-ttu-id="da058-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="da058-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="da058-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="da058-122">Authorization</span></span>  | <span data-ttu-id="da058-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da058-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da058-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da058-125">Request body</span></span>
<span data-ttu-id="da058-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da058-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da058-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="da058-127">Response</span></span>

<span data-ttu-id="da058-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da058-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da058-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da058-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da058-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da058-130">Request</span></span>
<span data-ttu-id="da058-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da058-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da058-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="da058-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da058-133">C#</span><span class="sxs-lookup"><span data-stu-id="da058-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da058-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da058-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da058-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="da058-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da058-136">Java</span><span class="sxs-lookup"><span data-stu-id="da058-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="da058-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="da058-137">Response</span></span>
<span data-ttu-id="da058-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da058-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
