---
title: Atualizar mailfolder
description: Atualize as propriedades do objeto mailfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 776fd98e7168793a81b9d2448c6dc823aaa36549
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025461"
---
# <a name="update-mailfolder"></a><span data-ttu-id="ff09e-103">Atualizar mailfolder</span><span class="sxs-lookup"><span data-stu-id="ff09e-103">Update mailfolder</span></span>

<span data-ttu-id="ff09e-104">Atualize as propriedades do objeto mailfolder.</span><span class="sxs-lookup"><span data-stu-id="ff09e-104">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff09e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff09e-105">Permissions</span></span>
<span data-ttu-id="ff09e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff09e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff09e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff09e-108">Permission type</span></span>      | <span data-ttu-id="ff09e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff09e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff09e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff09e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff09e-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff09e-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ff09e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff09e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff09e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff09e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ff09e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff09e-114">Application</span></span> | <span data-ttu-id="ff09e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff09e-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff09e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff09e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ff09e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff09e-117">Request headers</span></span>
| <span data-ttu-id="ff09e-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff09e-118">Header</span></span>       | <span data-ttu-id="ff09e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="ff09e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff09e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff09e-120">Authorization</span></span>  | <span data-ttu-id="ff09e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff09e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff09e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff09e-123">Content-Type</span></span>  | <span data-ttu-id="ff09e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff09e-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff09e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff09e-126">Request body</span></span>
<span data-ttu-id="ff09e-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ff09e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ff09e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff09e-130">Property</span></span>     | <span data-ttu-id="ff09e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff09e-131">Type</span></span>   |<span data-ttu-id="ff09e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff09e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff09e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ff09e-133">displayName</span></span>|<span data-ttu-id="ff09e-134">String</span><span class="sxs-lookup"><span data-stu-id="ff09e-134">String</span></span>|<span data-ttu-id="ff09e-135">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="ff09e-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="ff09e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff09e-136">Response</span></span>

<span data-ttu-id="ff09e-137">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff09e-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff09e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff09e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff09e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff09e-139">Request</span></span>
<span data-ttu-id="ff09e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff09e-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff09e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff09e-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff09e-142">C#</span><span class="sxs-lookup"><span data-stu-id="ff09e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff09e-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff09e-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff09e-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ff09e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff09e-145">Java</span><span class="sxs-lookup"><span data-stu-id="ff09e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ff09e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff09e-146">Response</span></span>
<span data-ttu-id="ff09e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff09e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
