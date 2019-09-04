---
title: 'privilegedRoleAssignment: My'
description: Obtenha as atribuições de função privilegiada do solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 948d0919e296824c32919bed50407579f2978bed
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725581"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="b7064-103">privilegedRoleAssignment: My</span><span class="sxs-lookup"><span data-stu-id="b7064-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7064-104">Obtenha as atribuições de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="b7064-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7064-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7064-105">Permissions</span></span>
<span data-ttu-id="b7064-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7064-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7064-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7064-108">Permission type</span></span>      | <span data-ttu-id="b7064-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7064-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7064-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7064-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7064-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b7064-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b7064-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7064-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7064-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7064-113">Not supported.</span></span>    |
|<span data-ttu-id="b7064-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7064-114">Application</span></span> | <span data-ttu-id="b7064-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7064-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7064-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7064-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="b7064-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7064-117">Request headers</span></span>
| <span data-ttu-id="b7064-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b7064-118">Name</span></span>       | <span data-ttu-id="b7064-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7064-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7064-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7064-120">Authorization</span></span>  | <span data-ttu-id="b7064-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7064-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7064-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7064-123">Request body</span></span>
<span data-ttu-id="b7064-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7064-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7064-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7064-125">Response</span></span>

<span data-ttu-id="b7064-126">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7064-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7064-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7064-127">Example</span></span>
<span data-ttu-id="b7064-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b7064-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7064-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7064-129">Request</span></span>
<span data-ttu-id="b7064-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7064-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b7064-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7064-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7064-132">C#</span><span class="sxs-lookup"><span data-stu-id="b7064-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7064-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7064-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7064-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b7064-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b7064-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7064-135">Response</span></span>
<span data-ttu-id="b7064-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7064-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
