---
title: Obter outlookTaskGroup
description: Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5840189cba9e340c9562315c5fbfcd3d76b7d416
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596204"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="f4284-103">Obter outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f4284-103">Get outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4284-104">Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f4284-104">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="f4284-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4284-105">Permissions</span></span>
<span data-ttu-id="f4284-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4284-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4284-108">Permission type</span></span>      | <span data-ttu-id="f4284-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4284-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4284-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4284-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f4284-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f4284-111">Tasks.Read</span></span>    |
|<span data-ttu-id="f4284-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4284-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4284-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f4284-113">Tasks.Read</span></span>    |
|<span data-ttu-id="f4284-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4284-114">Application</span></span> | <span data-ttu-id="f4284-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4284-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4284-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4284-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f4284-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f4284-117">Optional query parameters</span></span>
<span data-ttu-id="f4284-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f4284-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4284-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4284-119">Request headers</span></span>
| <span data-ttu-id="f4284-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f4284-120">Name</span></span>      |<span data-ttu-id="f4284-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4284-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f4284-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4284-122">Authorization</span></span>  | <span data-ttu-id="f4284-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4284-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4284-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4284-125">Request body</span></span>
<span data-ttu-id="f4284-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4284-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4284-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4284-127">Response</span></span>

<span data-ttu-id="f4284-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4284-128">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f4284-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4284-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4284-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4284-130">Request</span></span>
<span data-ttu-id="f4284-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4284-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
##### <a name="response"></a><span data-ttu-id="f4284-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4284-132">Response</span></span>
<span data-ttu-id="f4284-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4284-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f4284-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f4284-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f4284-137">Basic</span><span class="sxs-lookup"><span data-stu-id="f4284-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_outlooktaskgroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4284-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4284-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_outlooktaskgroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlooktaskgroup-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktaskgroup-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
