---
title: Obter outlookTaskFolder
description: Obtenha as propriedades e os relacionamentos da pasta de tarefas especificada do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 82e482f740b4292b723971e21682df32160a8a72
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723690"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="8b56f-103">Obter outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8b56f-103">Get outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b56f-104">Obtenha as propriedades e os relacionamentos da pasta de tarefas especificada do Outlook.</span><span class="sxs-lookup"><span data-stu-id="8b56f-104">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b56f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b56f-105">Permissions</span></span>
<span data-ttu-id="8b56f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b56f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b56f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b56f-108">Permission type</span></span>      | <span data-ttu-id="8b56f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b56f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b56f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b56f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b56f-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8b56f-111">Tasks.Read</span></span>    |
|<span data-ttu-id="8b56f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b56f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b56f-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8b56f-113">Tasks.Read</span></span>    |
|<span data-ttu-id="8b56f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b56f-114">Application</span></span> | <span data-ttu-id="8b56f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b56f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b56f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b56f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b56f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8b56f-117">Optional query parameters</span></span>
<span data-ttu-id="8b56f-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8b56f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b56f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b56f-119">Request headers</span></span>
| <span data-ttu-id="8b56f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8b56f-120">Name</span></span>      |<span data-ttu-id="8b56f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b56f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b56f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b56f-122">Authorization</span></span>  | <span data-ttu-id="8b56f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b56f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b56f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b56f-125">Request body</span></span>
<span data-ttu-id="8b56f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b56f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b56f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b56f-127">Response</span></span>

<span data-ttu-id="8b56f-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b56f-128">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b56f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b56f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b56f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b56f-130">Request</span></span>
<span data-ttu-id="8b56f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b56f-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8b56f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b56f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8b56f-133">C#</span><span class="sxs-lookup"><span data-stu-id="8b56f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b56f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b56f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8b56f-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8b56f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8b56f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b56f-136">Response</span></span>
<span data-ttu-id="8b56f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b56f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
