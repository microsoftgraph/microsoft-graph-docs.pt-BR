---
title: Excluir inferenceClassificationOverride
description: Exclua uma substituição especificada de acordo com sua ID.
localization_priority: Normal
ms.openlocfilehash: ae4043f0f118519de860c12431f0c6a80289a08f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277109"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="50ba8-103">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="50ba8-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="50ba8-104">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="50ba8-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="50ba8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="50ba8-105">Permissions</span></span>
<span data-ttu-id="50ba8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50ba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ba8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50ba8-108">Permission type</span></span>      | <span data-ttu-id="50ba8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50ba8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50ba8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50ba8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50ba8-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50ba8-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50ba8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50ba8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50ba8-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50ba8-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50ba8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50ba8-114">Application</span></span> | <span data-ttu-id="50ba8-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50ba8-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="50ba8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50ba8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="50ba8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50ba8-117">Request headers</span></span>
| <span data-ttu-id="50ba8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="50ba8-118">Name</span></span>       | <span data-ttu-id="50ba8-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="50ba8-119">Type</span></span> | <span data-ttu-id="50ba8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="50ba8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50ba8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50ba8-121">Authorization</span></span>  | <span data-ttu-id="50ba8-122">string</span><span class="sxs-lookup"><span data-stu-id="50ba8-122">string</span></span>  | <span data-ttu-id="50ba8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50ba8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50ba8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50ba8-125">Request body</span></span>
<span data-ttu-id="50ba8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50ba8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50ba8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="50ba8-127">Response</span></span>

<span data-ttu-id="50ba8-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50ba8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50ba8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50ba8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50ba8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50ba8-131">Request</span></span>
<span data-ttu-id="50ba8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50ba8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="50ba8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="50ba8-133">Response</span></span>
<span data-ttu-id="50ba8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50ba8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="50ba8-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="50ba8-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="50ba8-138">C#</span><span class="sxs-lookup"><span data-stu-id="50ba8-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50ba8-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="50ba8-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="50ba8-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="50ba8-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
