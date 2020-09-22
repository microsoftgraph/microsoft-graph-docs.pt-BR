---
title: Excluir inferenceClassificationOverride
description: Excluir uma substituição de caixa de entrada destaques especificada por sua ID.
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: ''
ms.openlocfilehash: 527670f84931c61f08151646780f8b8e6d95fcf0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001565"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="3c156-103">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="3c156-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="3c156-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c156-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c156-105">Excluir uma substituição de [caixa de entrada destaques](../resources/manage-focused-inbox.md) especificada por sua ID.</span><span class="sxs-lookup"><span data-stu-id="3c156-105">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c156-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c156-106">Permissions</span></span>
<span data-ttu-id="3c156-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c156-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c156-109">Permission type</span></span>      | <span data-ttu-id="3c156-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c156-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c156-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c156-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c156-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c156-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3c156-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c156-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c156-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c156-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3c156-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c156-115">Application</span></span> | <span data-ttu-id="3c156-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c156-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c156-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c156-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3c156-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c156-118">Request headers</span></span>
| <span data-ttu-id="3c156-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3c156-119">Name</span></span>       | <span data-ttu-id="3c156-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c156-120">Type</span></span> | <span data-ttu-id="3c156-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c156-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c156-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c156-122">Authorization</span></span>  | <span data-ttu-id="3c156-123">string</span><span class="sxs-lookup"><span data-stu-id="3c156-123">string</span></span>  | <span data-ttu-id="3c156-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c156-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c156-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c156-126">Request body</span></span>
<span data-ttu-id="3c156-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c156-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c156-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c156-128">Response</span></span>

<span data-ttu-id="3c156-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c156-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c156-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c156-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c156-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c156-132">Request</span></span>
<span data-ttu-id="3c156-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c156-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c156-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c156-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="c"></a>[<span data-ttu-id="3c156-135">C#</span><span class="sxs-lookup"><span data-stu-id="3c156-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c156-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c156-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c156-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c156-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c156-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c156-138">Response</span></span>
<span data-ttu-id="3c156-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c156-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


