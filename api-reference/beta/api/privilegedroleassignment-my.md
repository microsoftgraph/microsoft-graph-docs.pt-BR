---
title: 'privilegedRoleAssignment: my'
description: Obter as atribuições de função privilegiada do solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 71d683092ead996daff5cb86eba8ca02abe80192
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441190"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="29d18-103">privilegedRoleAssignment: my</span><span class="sxs-lookup"><span data-stu-id="29d18-103">privilegedRoleAssignment: my</span></span>

<span data-ttu-id="29d18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29d18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29d18-105">Obter as atribuições de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="29d18-105">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="29d18-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="29d18-106">Permissions</span></span>
<span data-ttu-id="29d18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29d18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29d18-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29d18-109">Permission type</span></span>      | <span data-ttu-id="29d18-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29d18-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29d18-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29d18-111">Delegated (work or school account)</span></span> | <span data-ttu-id="29d18-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29d18-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29d18-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29d18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29d18-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29d18-114">Not supported.</span></span>    |
|<span data-ttu-id="29d18-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29d18-115">Application</span></span> | <span data-ttu-id="29d18-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29d18-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29d18-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29d18-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="29d18-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29d18-118">Request headers</span></span>
| <span data-ttu-id="29d18-119">Nome</span><span class="sxs-lookup"><span data-stu-id="29d18-119">Name</span></span>       | <span data-ttu-id="29d18-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="29d18-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29d18-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="29d18-121">Authorization</span></span>  | <span data-ttu-id="29d18-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29d18-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29d18-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29d18-124">Request body</span></span>
<span data-ttu-id="29d18-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29d18-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29d18-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="29d18-126">Response</span></span>

<span data-ttu-id="29d18-127">Se tiver êxito, este método retornará o código de resposta e o objeto da coleção `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29d18-127">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29d18-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29d18-128">Example</span></span>
<span data-ttu-id="29d18-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="29d18-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="29d18-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29d18-130">Request</span></span>
<span data-ttu-id="29d18-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29d18-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29d18-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="29d18-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```
# <a name="c"></a>[<span data-ttu-id="29d18-133">C#</span><span class="sxs-lookup"><span data-stu-id="29d18-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29d18-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29d18-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29d18-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29d18-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29d18-136">Java</span><span class="sxs-lookup"><span data-stu-id="29d18-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-my-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="29d18-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="29d18-137">Response</span></span>
<span data-ttu-id="29d18-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29d18-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


