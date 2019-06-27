---
title: Create privilegedApproval
description: Use esta API para criar um novo privilegedApproval.
localization_priority: Normal
ms.openlocfilehash: 25f11589304ddaf1d5e2fc21bb787b17fab4f1fa
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268170"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="fdb1f-103">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="fdb1f-103">Create privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdb1f-104">Use esta API para criar um novo privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="fdb1f-104">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="fdb1f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdb1f-105">Permissions</span></span>
<span data-ttu-id="fdb1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdb1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fdb1f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdb1f-108">Permission type</span></span>      | <span data-ttu-id="fdb1f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdb1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdb1f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdb1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fdb1f-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fdb1f-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fdb1f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdb1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdb1f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdb1f-113">Not supported.</span></span>    |
|<span data-ttu-id="fdb1f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdb1f-114">Application</span></span> | <span data-ttu-id="fdb1f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdb1f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdb1f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdb1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="fdb1f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb1f-117">Request headers</span></span>
| <span data-ttu-id="fdb1f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fdb1f-118">Name</span></span>       | <span data-ttu-id="fdb1f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdb1f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fdb1f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdb1f-120">Authorization</span></span>  | <span data-ttu-id="fdb1f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdb1f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdb1f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb1f-123">Request body</span></span>
<span data-ttu-id="fdb1f-124">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="fdb1f-124">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fdb1f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb1f-125">Response</span></span>

<span data-ttu-id="fdb1f-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdb1f-126">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="fdb1f-127">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="fdb1f-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="fdb1f-128">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="fdb1f-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="fdb1f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdb1f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fdb1f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb1f-130">Request</span></span>
<span data-ttu-id="fdb1f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdb1f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
<span data-ttu-id="fdb1f-132">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="fdb1f-132">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fdb1f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb1f-133">Response</span></span>
<span data-ttu-id="fdb1f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdb1f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fdb1f-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fdb1f-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fdb1f-138">C#</span><span class="sxs-lookup"><span data-stu-id="fdb1f-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_privilegedapproval_from_privilegedapproval-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fdb1f-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="fdb1f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_privilegedapproval_from_privilegedapproval-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fdb1f-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fdb1f-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_privilegedapproval_from_privilegedapproval-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
