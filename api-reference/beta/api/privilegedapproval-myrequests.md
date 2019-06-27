---
title: 'privilegedApproval: myrequests'
description: Receba solicitações de aprovação do solicitante.
localization_priority: Normal
ms.openlocfilehash: 71c9ffd79a48df0e4c9bc9fa84c9f61dca1a0594
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267722"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="a7a97-103">privilegedApproval: myrequests</span><span class="sxs-lookup"><span data-stu-id="a7a97-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7a97-104">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="a7a97-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7a97-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7a97-105">Permissions</span></span>
<span data-ttu-id="a7a97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7a97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a7a97-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7a97-108">Permission type</span></span>      | <span data-ttu-id="a7a97-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7a97-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7a97-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7a97-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7a97-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7a97-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a7a97-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7a97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7a97-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7a97-113">Not supported.</span></span>    |
|<span data-ttu-id="a7a97-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7a97-114">Application</span></span> | <span data-ttu-id="a7a97-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7a97-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7a97-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7a97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="a7a97-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7a97-117">Request headers</span></span>
| <span data-ttu-id="a7a97-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a7a97-118">Name</span></span>       | <span data-ttu-id="a7a97-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7a97-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7a97-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7a97-120">Authorization</span></span>  | <span data-ttu-id="a7a97-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7a97-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7a97-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7a97-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a7a97-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7a97-124">Response</span></span>

<span data-ttu-id="a7a97-125">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7a97-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="a7a97-126">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="a7a97-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a7a97-127">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="a7a97-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="a7a97-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7a97-128">Example</span></span>
<span data-ttu-id="a7a97-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a7a97-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a7a97-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7a97-130">Request</span></span>
<span data-ttu-id="a7a97-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7a97-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="a7a97-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7a97-132">Response</span></span>
<span data-ttu-id="a7a97-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7a97-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a7a97-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a7a97-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a7a97-137">C#</span><span class="sxs-lookup"><span data-stu-id="a7a97-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedapproval_myrequests-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7a97-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7a97-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedapproval_myrequests-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a7a97-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a7a97-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/privilegedapproval_myrequests-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
