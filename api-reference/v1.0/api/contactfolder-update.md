---
title: Atualizar contactfolder
description: Atualiza as propriedades do objeto contactfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7e3940bc1f9a1d46efc04bbb8d608f8693953855
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365787"
---
# <a name="update-contactfolder"></a><span data-ttu-id="63ff9-103">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="63ff9-103">Update contactfolder</span></span>

<span data-ttu-id="63ff9-104">Atualiza as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="63ff9-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="63ff9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="63ff9-105">Permissions</span></span>
<span data-ttu-id="63ff9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63ff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63ff9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63ff9-108">Permission type</span></span>      | <span data-ttu-id="63ff9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63ff9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63ff9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63ff9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63ff9-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63ff9-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="63ff9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63ff9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63ff9-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63ff9-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="63ff9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63ff9-114">Application</span></span> | <span data-ttu-id="63ff9-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63ff9-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="63ff9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63ff9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="63ff9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63ff9-117">Request headers</span></span>
| <span data-ttu-id="63ff9-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63ff9-118">Header</span></span>       | <span data-ttu-id="63ff9-119">Valor</span><span class="sxs-lookup"><span data-stu-id="63ff9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63ff9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="63ff9-120">Authorization</span></span>  | <span data-ttu-id="63ff9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63ff9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="63ff9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63ff9-123">Content-Type</span></span>  | <span data-ttu-id="63ff9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63ff9-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63ff9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63ff9-126">Request body</span></span>
<span data-ttu-id="63ff9-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="63ff9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="63ff9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63ff9-130">Property</span></span>     | <span data-ttu-id="63ff9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="63ff9-131">Type</span></span>   |<span data-ttu-id="63ff9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="63ff9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63ff9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="63ff9-133">displayName</span></span>|<span data-ttu-id="63ff9-134">String</span><span class="sxs-lookup"><span data-stu-id="63ff9-134">String</span></span>|<span data-ttu-id="63ff9-135">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="63ff9-135">The folder's display name.</span></span>|
|<span data-ttu-id="63ff9-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="63ff9-136">parentFolderId</span></span>|<span data-ttu-id="63ff9-137">String</span><span class="sxs-lookup"><span data-stu-id="63ff9-137">String</span></span>|<span data-ttu-id="63ff9-138">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="63ff9-138">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="63ff9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="63ff9-139">Response</span></span>

<span data-ttu-id="63ff9-140">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63ff9-140">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="63ff9-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63ff9-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63ff9-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63ff9-142">Request</span></span>
<span data-ttu-id="63ff9-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63ff9-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63ff9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="63ff9-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="63ff9-145">C#</span><span class="sxs-lookup"><span data-stu-id="63ff9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63ff9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63ff9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63ff9-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="63ff9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="63ff9-148">Java</span><span class="sxs-lookup"><span data-stu-id="63ff9-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="63ff9-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="63ff9-149">Response</span></span>
<span data-ttu-id="63ff9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63ff9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
