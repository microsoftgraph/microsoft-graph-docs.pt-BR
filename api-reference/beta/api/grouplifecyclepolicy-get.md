---
title: Obter groupLifecyclePolicy
description: Recupera as propriedades e os relacionamentos de um objeto groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3b5dba23c42f9bfe175875399eceeb4e8870fc9c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592354"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="d2219-103">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d2219-103">Get groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2219-104">Recupera as propriedades e os relacionamentos de um objeto [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d2219-104">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2219-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2219-105">Permissions</span></span>

<span data-ttu-id="d2219-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d2219-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2219-108">Permission type</span></span>      | <span data-ttu-id="d2219-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2219-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2219-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2219-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2219-111">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2219-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d2219-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2219-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2219-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d2219-113">Not supported</span></span> |
|<span data-ttu-id="d2219-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2219-114">Application</span></span> | <span data-ttu-id="d2219-115">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2219-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2219-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2219-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2219-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2219-117">Optional query parameters</span></span>
<span data-ttu-id="d2219-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2219-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2219-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2219-119">Request headers</span></span>
| <span data-ttu-id="d2219-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d2219-120">Name</span></span> | <span data-ttu-id="d2219-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2219-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="d2219-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2219-122">Authorization</span></span> | <span data-ttu-id="d2219-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2219-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2219-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2219-125">Request body</span></span>
<span data-ttu-id="d2219-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2219-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d2219-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2219-127">Response</span></span>
<span data-ttu-id="d2219-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2219-128">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2219-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2219-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d2219-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2219-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="d2219-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2219-131">Response</span></span>

<span data-ttu-id="d2219-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2219-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d2219-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d2219-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d2219-135">Basic</span><span class="sxs-lookup"><span data-stu-id="d2219-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2219-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2219-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicy-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
