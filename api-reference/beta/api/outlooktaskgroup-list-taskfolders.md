---
title: Listar taskFolders
description: Obter pastas de tarefas do Outlook em um outlookTaskGroup específico.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1753a2bfe73c92d098c9f5201f70479975445635
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447226"
---
# <a name="list-taskfolders"></a><span data-ttu-id="ab68b-103">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="ab68b-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab68b-104">Obter pastas de tarefas do Outlook em um [outlookTaskGroup](../resources/outlooktaskgroup.md)específico.</span><span class="sxs-lookup"><span data-stu-id="ab68b-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ab68b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab68b-105">Permissions</span></span>
<span data-ttu-id="ab68b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab68b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab68b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab68b-108">Permission type</span></span>      | <span data-ttu-id="ab68b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab68b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab68b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab68b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab68b-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ab68b-111">Tasks.Read</span></span>    |
|<span data-ttu-id="ab68b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab68b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab68b-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ab68b-113">Tasks.Read</span></span>    |
|<span data-ttu-id="ab68b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab68b-114">Application</span></span> | <span data-ttu-id="ab68b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab68b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab68b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab68b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab68b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab68b-117">Optional query parameters</span></span>
<span data-ttu-id="ab68b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab68b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab68b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab68b-119">Request headers</span></span>
| <span data-ttu-id="ab68b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ab68b-120">Name</span></span>      |<span data-ttu-id="ab68b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab68b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab68b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab68b-122">Authorization</span></span>  | <span data-ttu-id="ab68b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab68b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab68b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab68b-125">Request body</span></span>
<span data-ttu-id="ab68b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab68b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab68b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab68b-127">Response</span></span>

<span data-ttu-id="ab68b-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab68b-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab68b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab68b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab68b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab68b-130">Request</span></span>
<span data-ttu-id="ab68b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab68b-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ab68b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab68b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ab68b-133">C#</span><span class="sxs-lookup"><span data-stu-id="ab68b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab68b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ab68b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ab68b-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ab68b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ab68b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab68b-136">Response</span></span>
<span data-ttu-id="ab68b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab68b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
