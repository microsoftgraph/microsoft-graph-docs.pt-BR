---
title: 'privilegedRoleAssignment: My'
description: Obtenha as atribuições de função privilegiada do solicitante.
localization_priority: Normal
ms.openlocfilehash: 4d4b1c9df882c89ccd4b10d0dcaa904d060273fb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264173"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="2510e-103">privilegedRoleAssignment: My</span><span class="sxs-lookup"><span data-stu-id="2510e-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2510e-104">Obtenha as atribuições de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="2510e-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="2510e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2510e-105">Permissions</span></span>
<span data-ttu-id="2510e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2510e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2510e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2510e-108">Permission type</span></span>      | <span data-ttu-id="2510e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2510e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2510e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2510e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2510e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2510e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2510e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2510e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2510e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2510e-113">Not supported.</span></span>    |
|<span data-ttu-id="2510e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2510e-114">Application</span></span> | <span data-ttu-id="2510e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2510e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2510e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2510e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="2510e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2510e-117">Request headers</span></span>
| <span data-ttu-id="2510e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2510e-118">Name</span></span>       | <span data-ttu-id="2510e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2510e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2510e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2510e-120">Authorization</span></span>  | <span data-ttu-id="2510e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2510e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2510e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2510e-123">Request body</span></span>
<span data-ttu-id="2510e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2510e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2510e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2510e-125">Response</span></span>

<span data-ttu-id="2510e-126">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2510e-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2510e-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2510e-127">Example</span></span>
<span data-ttu-id="2510e-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2510e-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2510e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2510e-129">Request</span></span>
<span data-ttu-id="2510e-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2510e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="2510e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2510e-131">Response</span></span>
<span data-ttu-id="2510e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2510e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2510e-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2510e-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2510e-136">C#</span><span class="sxs-lookup"><span data-stu-id="2510e-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_my-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2510e-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="2510e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_my-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2510e-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2510e-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_my-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignment-my.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-my.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-my.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
