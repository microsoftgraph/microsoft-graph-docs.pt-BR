---
title: Atualizar mailFolder
description: Atualize as propriedades do objeto mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 022c992dedb8dc06f3a17b58f0ec5e96b0f1d0b3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415194"
---
# <a name="update-mailfolder"></a><span data-ttu-id="94aa1-103">Atualizar mailFolder</span><span class="sxs-lookup"><span data-stu-id="94aa1-103">Update mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94aa1-104">Atualize as propriedades do objeto [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="94aa1-104">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94aa1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="94aa1-105">Permissions</span></span>
<span data-ttu-id="94aa1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94aa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94aa1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94aa1-108">Permission type</span></span>      | <span data-ttu-id="94aa1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94aa1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94aa1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94aa1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94aa1-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94aa1-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94aa1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94aa1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94aa1-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94aa1-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94aa1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94aa1-114">Application</span></span> | <span data-ttu-id="94aa1-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94aa1-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94aa1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94aa1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94aa1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94aa1-117">Request headers</span></span>
| <span data-ttu-id="94aa1-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94aa1-118">Header</span></span>       | <span data-ttu-id="94aa1-119">Valor</span><span class="sxs-lookup"><span data-stu-id="94aa1-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94aa1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="94aa1-120">Authorization</span></span>  | <span data-ttu-id="94aa1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94aa1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94aa1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94aa1-123">Content-Type</span></span>  | <span data-ttu-id="94aa1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94aa1-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94aa1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94aa1-126">Request body</span></span>
<span data-ttu-id="94aa1-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="94aa1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94aa1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94aa1-130">Property</span></span>     | <span data-ttu-id="94aa1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="94aa1-131">Type</span></span>   |<span data-ttu-id="94aa1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="94aa1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94aa1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="94aa1-133">displayName</span></span>|<span data-ttu-id="94aa1-134">String</span><span class="sxs-lookup"><span data-stu-id="94aa1-134">String</span></span>|<span data-ttu-id="94aa1-135">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="94aa1-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="94aa1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="94aa1-136">Response</span></span>
<span data-ttu-id="94aa1-137">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94aa1-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94aa1-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94aa1-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="94aa1-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94aa1-139">Request</span></span>
<span data-ttu-id="94aa1-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94aa1-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94aa1-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="94aa1-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94aa1-142">C#</span><span class="sxs-lookup"><span data-stu-id="94aa1-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94aa1-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94aa1-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94aa1-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="94aa1-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94aa1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="94aa1-145">Response</span></span>
<span data-ttu-id="94aa1-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94aa1-146">The following is an example of the response.</span></span>
><span data-ttu-id="94aa1-147">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="94aa1-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="94aa1-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94aa1-148">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
