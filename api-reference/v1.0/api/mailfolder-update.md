---
title: Atualizar mailfolder
description: Atualize as propriedades do objeto mailfolder.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3842eba43eee73c789669978d770075f4979158a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136132"
---
# <a name="update-mailfolder"></a><span data-ttu-id="55722-103">Atualizar mailfolder</span><span class="sxs-lookup"><span data-stu-id="55722-103">Update mailfolder</span></span>

<span data-ttu-id="55722-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55722-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55722-105">Atualize as propriedades do objeto mailfolder.</span><span class="sxs-lookup"><span data-stu-id="55722-105">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="55722-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="55722-106">Permissions</span></span>
<span data-ttu-id="55722-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55722-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55722-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55722-109">Permission type</span></span>      | <span data-ttu-id="55722-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55722-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55722-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55722-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55722-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55722-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="55722-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55722-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55722-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55722-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="55722-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55722-115">Application</span></span> | <span data-ttu-id="55722-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55722-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="55722-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55722-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="55722-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55722-118">Request headers</span></span>
| <span data-ttu-id="55722-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55722-119">Header</span></span>       | <span data-ttu-id="55722-120">Valor</span><span class="sxs-lookup"><span data-stu-id="55722-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55722-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="55722-121">Authorization</span></span>  | <span data-ttu-id="55722-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55722-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="55722-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55722-124">Content-Type</span></span>  | <span data-ttu-id="55722-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55722-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55722-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55722-127">Request body</span></span>
<span data-ttu-id="55722-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="55722-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="55722-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55722-131">Property</span></span>     | <span data-ttu-id="55722-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="55722-132">Type</span></span>   |<span data-ttu-id="55722-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="55722-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55722-134">displayName</span><span class="sxs-lookup"><span data-stu-id="55722-134">displayName</span></span>|<span data-ttu-id="55722-135">String</span><span class="sxs-lookup"><span data-stu-id="55722-135">String</span></span>|<span data-ttu-id="55722-136">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="55722-136">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="55722-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="55722-137">Response</span></span>

<span data-ttu-id="55722-138">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55722-138">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55722-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55722-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55722-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55722-140">Request</span></span>
<span data-ttu-id="55722-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55722-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55722-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="55722-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="55722-143">C#</span><span class="sxs-lookup"><span data-stu-id="55722-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55722-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55722-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55722-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55722-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55722-146">Java</span><span class="sxs-lookup"><span data-stu-id="55722-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="55722-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="55722-147">Response</span></span>
<span data-ttu-id="55722-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55722-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

