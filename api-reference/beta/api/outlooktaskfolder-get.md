---
title: Obter outlookTaskFolder
description: Obter as propriedades e as relações da pasta de tarefas Outlook especificada.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f6de43ed163c49a52df82df4368eca1aff1e51f8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055453"
---
# <a name="get-outlooktaskfolder-deprecated"></a><span data-ttu-id="c2ef0-103">Obter outlookTaskFolder (preterido)</span><span class="sxs-lookup"><span data-stu-id="c2ef0-103">Get outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="c2ef0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2ef0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="c2ef0-105">Obter as propriedades e as relações da pasta de tarefas Outlook especificada.</span><span class="sxs-lookup"><span data-stu-id="c2ef0-105">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2ef0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2ef0-106">Permissions</span></span>
<span data-ttu-id="c2ef0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2ef0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2ef0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2ef0-109">Permission type</span></span>      | <span data-ttu-id="c2ef0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2ef0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2ef0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2ef0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2ef0-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c2ef0-112">Tasks.Read</span></span>    |
|<span data-ttu-id="c2ef0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2ef0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2ef0-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c2ef0-114">Tasks.Read</span></span>    |
|<span data-ttu-id="c2ef0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2ef0-115">Application</span></span> | <span data-ttu-id="c2ef0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2ef0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2ef0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2ef0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2ef0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2ef0-118">Optional query parameters</span></span>
<span data-ttu-id="c2ef0-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c2ef0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2ef0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2ef0-120">Request headers</span></span>
| <span data-ttu-id="c2ef0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c2ef0-121">Name</span></span>      |<span data-ttu-id="c2ef0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2ef0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2ef0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2ef0-123">Authorization</span></span>  | <span data-ttu-id="c2ef0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2ef0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2ef0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2ef0-126">Request body</span></span>
<span data-ttu-id="c2ef0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2ef0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2ef0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2ef0-128">Response</span></span>

<span data-ttu-id="c2ef0-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2ef0-129">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2ef0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2ef0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2ef0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2ef0-131">Request</span></span>
<span data-ttu-id="c2ef0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2ef0-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2ef0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2ef0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="c2ef0-134">C#</span><span class="sxs-lookup"><span data-stu-id="c2ef0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2ef0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2ef0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2ef0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2ef0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2ef0-137">Java</span><span class="sxs-lookup"><span data-stu-id="c2ef0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktaskfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2ef0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2ef0-138">Response</span></span>
<span data-ttu-id="c2ef0-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2ef0-139">Here is an example of the response.</span></span> <span data-ttu-id="c2ef0-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c2ef0-140">Note: The response object shown here might be shortened for readability.</span></span>
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
