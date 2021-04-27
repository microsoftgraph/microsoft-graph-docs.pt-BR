---
title: Atualizar mailFolder
description: Atualize as propriedades do objeto mailFolder.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b6039bf189d88c46612fab8ec71ac6ae4eb7909b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053003"
---
# <a name="update-mailfolder"></a><span data-ttu-id="616dc-103">Atualizar mailFolder</span><span class="sxs-lookup"><span data-stu-id="616dc-103">Update mailFolder</span></span>

<span data-ttu-id="616dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="616dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="616dc-105">Atualize as propriedades do [objeto mailFolder.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="616dc-105">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="616dc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="616dc-106">Permissions</span></span>
<span data-ttu-id="616dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="616dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="616dc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="616dc-109">Permission type</span></span>      | <span data-ttu-id="616dc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="616dc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="616dc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="616dc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="616dc-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="616dc-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="616dc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="616dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="616dc-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="616dc-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="616dc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="616dc-115">Application</span></span> | <span data-ttu-id="616dc-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="616dc-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="616dc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="616dc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="616dc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="616dc-118">Request headers</span></span>
| <span data-ttu-id="616dc-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="616dc-119">Header</span></span>       | <span data-ttu-id="616dc-120">Valor</span><span class="sxs-lookup"><span data-stu-id="616dc-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="616dc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="616dc-121">Authorization</span></span>  | <span data-ttu-id="616dc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="616dc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="616dc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="616dc-124">Content-Type</span></span>  | <span data-ttu-id="616dc-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="616dc-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="616dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="616dc-127">Request body</span></span>
<span data-ttu-id="616dc-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="616dc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="616dc-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="616dc-131">Property</span></span>     | <span data-ttu-id="616dc-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="616dc-132">Type</span></span>   |<span data-ttu-id="616dc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="616dc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="616dc-134">displayName</span><span class="sxs-lookup"><span data-stu-id="616dc-134">displayName</span></span>|<span data-ttu-id="616dc-135">String</span><span class="sxs-lookup"><span data-stu-id="616dc-135">String</span></span>|<span data-ttu-id="616dc-136">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="616dc-136">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="616dc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="616dc-137">Response</span></span>
<span data-ttu-id="616dc-138">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="616dc-138">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="616dc-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="616dc-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="616dc-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="616dc-140">Request</span></span>
<span data-ttu-id="616dc-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="616dc-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="616dc-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="616dc-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="616dc-143">C#</span><span class="sxs-lookup"><span data-stu-id="616dc-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="616dc-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="616dc-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="616dc-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="616dc-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="616dc-146">Java</span><span class="sxs-lookup"><span data-stu-id="616dc-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="616dc-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="616dc-147">Response</span></span>
<span data-ttu-id="616dc-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="616dc-148">The following is an example of the response.</span></span>
><span data-ttu-id="616dc-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="616dc-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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


