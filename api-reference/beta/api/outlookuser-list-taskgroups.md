---
title: Listar taskGroups
description: Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0bfaa943eaffa50ede1c78ee429fafc76b28dc19
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596260"
---
# <a name="list-taskgroups"></a><span data-ttu-id="2fb1b-103">Listar taskGroups</span><span class="sxs-lookup"><span data-stu-id="2fb1b-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fb1b-104">Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2fb1b-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="2fb1b-105">A resposta sempre inclui o grupo de tarefas padrão `My Tasks` e quaisquer outros grupos de tarefas criados na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2fb1b-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="2fb1b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fb1b-106">Permissions</span></span>
<span data-ttu-id="2fb1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fb1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fb1b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fb1b-109">Permission type</span></span>      | <span data-ttu-id="2fb1b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fb1b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fb1b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fb1b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2fb1b-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2fb1b-112">Tasks.Read</span></span>    |
|<span data-ttu-id="2fb1b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fb1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fb1b-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2fb1b-114">Tasks.Read</span></span>    |
|<span data-ttu-id="2fb1b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fb1b-115">Application</span></span> | <span data-ttu-id="2fb1b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fb1b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fb1b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fb1b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2fb1b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2fb1b-118">Optional query parameters</span></span>
<span data-ttu-id="2fb1b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2fb1b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2fb1b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fb1b-120">Request headers</span></span>
| <span data-ttu-id="2fb1b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2fb1b-121">Name</span></span>      |<span data-ttu-id="2fb1b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fb1b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2fb1b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fb1b-123">Authorization</span></span>  | <span data-ttu-id="2fb1b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fb1b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fb1b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fb1b-126">Request body</span></span>
<span data-ttu-id="2fb1b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2fb1b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fb1b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fb1b-128">Response</span></span>

<span data-ttu-id="2fb1b-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fb1b-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fb1b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fb1b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fb1b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fb1b-131">Request</span></span>
<span data-ttu-id="2fb1b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fb1b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="2fb1b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fb1b-133">Response</span></span>
<span data-ttu-id="2fb1b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fb1b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2fb1b-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2fb1b-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2fb1b-138">Basic</span><span class="sxs-lookup"><span data-stu-id="2fb1b-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_taskgroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fb1b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fb1b-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_taskgroups-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/outlookuser-list-taskgroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-list-taskgroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
