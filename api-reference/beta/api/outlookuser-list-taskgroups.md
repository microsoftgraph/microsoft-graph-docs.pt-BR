---
title: Listar taskGroups
description: Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: a086e45411a99bcd8f5a97ea7f1bb59a8542b320
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267792"
---
# <a name="list-taskgroups"></a><span data-ttu-id="c6f4f-103">Listar taskGroups</span><span class="sxs-lookup"><span data-stu-id="c6f4f-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6f4f-104">Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6f4f-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="c6f4f-105">A resposta sempre inclui o grupo de tarefas padrão `My Tasks` e quaisquer outros grupos de tarefas criados na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c6f4f-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6f4f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6f4f-106">Permissions</span></span>
<span data-ttu-id="c6f4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6f4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6f4f-109">Permission type</span></span>      | <span data-ttu-id="c6f4f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6f4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6f4f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6f4f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6f4f-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c6f4f-112">Tasks.Read</span></span>    |
|<span data-ttu-id="c6f4f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6f4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6f4f-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c6f4f-114">Tasks.Read</span></span>    |
|<span data-ttu-id="c6f4f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6f4f-115">Application</span></span> | <span data-ttu-id="c6f4f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6f4f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6f4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6f4f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6f4f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c6f4f-118">Optional query parameters</span></span>
<span data-ttu-id="c6f4f-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c6f4f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6f4f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6f4f-120">Request headers</span></span>
| <span data-ttu-id="c6f4f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c6f4f-121">Name</span></span>      |<span data-ttu-id="c6f4f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6f4f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c6f4f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6f4f-123">Authorization</span></span>  | <span data-ttu-id="c6f4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6f4f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6f4f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6f4f-126">Request body</span></span>
<span data-ttu-id="c6f4f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6f4f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6f4f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6f4f-128">Response</span></span>

<span data-ttu-id="c6f4f-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6f4f-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6f4f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6f4f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6f4f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6f4f-131">Request</span></span>
<span data-ttu-id="c6f4f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6f4f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="c6f4f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6f4f-133">Response</span></span>
<span data-ttu-id="c6f4f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6f4f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "id": "AAMkADIyAAADJ5pYAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxLA==",
      "isDefaultGroup": true,
      "name": "My Tasks",
      "groupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAhrbe-AAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
      "isDefaultGroup": false,
      "name": "Leisure Tasks",
      "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6f4f-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c6f4f-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6f4f-138">C#</span><span class="sxs-lookup"><span data-stu-id="c6f4f-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_taskgroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6f4f-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6f4f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_taskgroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6f4f-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c6f4f-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_taskgroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-taskgroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-list-taskgroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-list-taskgroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
