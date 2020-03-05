---
title: Listar taskFolders
description: Obter todas as pastas de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c671ffccbf6631a03fe3867ccecc4e54e91f8a3a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456079"
---
# <a name="list-taskfolders"></a><span data-ttu-id="59aaa-103">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="59aaa-103">List taskFolders</span></span>

<span data-ttu-id="59aaa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="59aaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59aaa-105">Obter todas as pastas de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="59aaa-105">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="59aaa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59aaa-106">Permissions</span></span>
<span data-ttu-id="59aaa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59aaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59aaa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59aaa-109">Permission type</span></span>      | <span data-ttu-id="59aaa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59aaa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59aaa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59aaa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59aaa-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="59aaa-112">Tasks.Read</span></span>    |
|<span data-ttu-id="59aaa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59aaa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59aaa-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="59aaa-114">Tasks.Read</span></span>    |
|<span data-ttu-id="59aaa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59aaa-115">Application</span></span> | <span data-ttu-id="59aaa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59aaa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59aaa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59aaa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59aaa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59aaa-118">Optional query parameters</span></span>
<span data-ttu-id="59aaa-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59aaa-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59aaa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59aaa-120">Request headers</span></span>
| <span data-ttu-id="59aaa-121">Nome</span><span class="sxs-lookup"><span data-stu-id="59aaa-121">Name</span></span>      |<span data-ttu-id="59aaa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="59aaa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59aaa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59aaa-123">Authorization</span></span>  | <span data-ttu-id="59aaa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59aaa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59aaa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59aaa-126">Request body</span></span>
<span data-ttu-id="59aaa-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59aaa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59aaa-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="59aaa-128">Response</span></span>

<span data-ttu-id="59aaa-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59aaa-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59aaa-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59aaa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59aaa-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59aaa-131">Request</span></span>
<span data-ttu-id="59aaa-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59aaa-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59aaa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="59aaa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
# <a name="c"></a>[<span data-ttu-id="59aaa-134">C#</span><span class="sxs-lookup"><span data-stu-id="59aaa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59aaa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59aaa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59aaa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59aaa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59aaa-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="59aaa-137">Response</span></span>
<span data-ttu-id="59aaa-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59aaa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADIyAAAAABrJAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
      "isDefaultFolder": false,
      "name": "Monthly tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAAAAESAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAAPA==",
      "isDefaultFolder": true,
      "name": "Tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TaskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
