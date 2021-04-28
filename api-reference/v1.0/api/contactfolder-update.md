---
title: Atualizar contactfolder
description: Atualiza as propriedades do objeto contactfolder.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b0dca141622a784702a2a2153774d8564d4ccc55
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035712"
---
# <a name="update-contactfolder"></a><span data-ttu-id="5d0cf-103">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="5d0cf-103">Update contactfolder</span></span>

<span data-ttu-id="5d0cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d0cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d0cf-105">Atualiza as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-105">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d0cf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d0cf-106">Permissions</span></span>
<span data-ttu-id="5d0cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d0cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d0cf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d0cf-109">Permission type</span></span>      | <span data-ttu-id="5d0cf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d0cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d0cf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d0cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d0cf-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d0cf-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5d0cf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d0cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d0cf-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d0cf-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5d0cf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d0cf-115">Application</span></span> | <span data-ttu-id="5d0cf-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d0cf-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d0cf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d0cf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5d0cf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d0cf-118">Request headers</span></span>
| <span data-ttu-id="5d0cf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d0cf-119">Header</span></span>       | <span data-ttu-id="5d0cf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5d0cf-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d0cf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d0cf-121">Authorization</span></span>  | <span data-ttu-id="5d0cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5d0cf-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d0cf-124">Content-Type</span></span>  | <span data-ttu-id="5d0cf-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d0cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d0cf-127">Request body</span></span>
<span data-ttu-id="5d0cf-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5d0cf-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d0cf-131">Property</span></span>     | <span data-ttu-id="5d0cf-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d0cf-132">Type</span></span>   |<span data-ttu-id="5d0cf-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d0cf-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d0cf-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5d0cf-134">displayName</span></span>|<span data-ttu-id="5d0cf-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d0cf-135">String</span></span>|<span data-ttu-id="5d0cf-136">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-136">The folder's display name.</span></span>|
|<span data-ttu-id="5d0cf-137">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="5d0cf-137">parentFolderId</span></span>|<span data-ttu-id="5d0cf-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d0cf-138">String</span></span>|<span data-ttu-id="5d0cf-139">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-139">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="5d0cf-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d0cf-140">Response</span></span>

<span data-ttu-id="5d0cf-141">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-141">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d0cf-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d0cf-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d0cf-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d0cf-143">Request</span></span>
<span data-ttu-id="5d0cf-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d0cf-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d0cf-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5d0cf-146">C#</span><span class="sxs-lookup"><span data-stu-id="5d0cf-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d0cf-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d0cf-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d0cf-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d0cf-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d0cf-149">Java</span><span class="sxs-lookup"><span data-stu-id="5d0cf-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5d0cf-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d0cf-150">Response</span></span>
<span data-ttu-id="5d0cf-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-151">Here is an example of the response.</span></span> <span data-ttu-id="5d0cf-152">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5d0cf-152">Note: The response object shown here might be shortened for readability.</span></span>
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

