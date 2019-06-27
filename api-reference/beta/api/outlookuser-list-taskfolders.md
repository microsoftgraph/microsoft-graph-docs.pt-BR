---
title: Listar taskFolders
description: Obter todas as pastas de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 023ab5b354c7159edfbf1ebc7789fb4f06c183b8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265727"
---
# <a name="list-taskfolders"></a><span data-ttu-id="fe08c-103">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="fe08c-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe08c-104">Obter todas as pastas de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="fe08c-104">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe08c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe08c-105">Permissions</span></span>
<span data-ttu-id="fe08c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe08c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe08c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe08c-108">Permission type</span></span>      | <span data-ttu-id="fe08c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe08c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe08c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe08c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe08c-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fe08c-111">Tasks.Read</span></span>    |
|<span data-ttu-id="fe08c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe08c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe08c-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fe08c-113">Tasks.Read</span></span>    |
|<span data-ttu-id="fe08c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe08c-114">Application</span></span> | <span data-ttu-id="fe08c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe08c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe08c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe08c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe08c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe08c-117">Optional query parameters</span></span>
<span data-ttu-id="fe08c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe08c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe08c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe08c-119">Request headers</span></span>
| <span data-ttu-id="fe08c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fe08c-120">Name</span></span>      |<span data-ttu-id="fe08c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe08c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe08c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe08c-122">Authorization</span></span>  | <span data-ttu-id="fe08c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe08c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe08c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe08c-125">Request body</span></span>
<span data-ttu-id="fe08c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe08c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe08c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe08c-127">Response</span></span>

<span data-ttu-id="fe08c-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe08c-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe08c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe08c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe08c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe08c-130">Request</span></span>
<span data-ttu-id="fe08c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe08c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
##### <a name="response"></a><span data-ttu-id="fe08c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe08c-132">Response</span></span>
<span data-ttu-id="fe08c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe08c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fe08c-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fe08c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fe08c-137">C#</span><span class="sxs-lookup"><span data-stu-id="fe08c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_taskfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe08c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="fe08c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_taskfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fe08c-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fe08c-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_taskfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlookuser-list-taskfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-list-taskfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-list-taskfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
