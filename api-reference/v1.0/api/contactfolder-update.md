---
title: Atualizar contactfolder
description: Atualiza as propriedades do objeto contactfolder.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3ff8c5a0532db0dc9d35902ffd76e26695ccfdcf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467648"
---
# <a name="update-contactfolder"></a><span data-ttu-id="10d0e-103">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="10d0e-103">Update contactfolder</span></span>

<span data-ttu-id="10d0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10d0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10d0e-105">Atualiza as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="10d0e-105">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="10d0e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10d0e-106">Permissions</span></span>
<span data-ttu-id="10d0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10d0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10d0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10d0e-109">Permission type</span></span>      | <span data-ttu-id="10d0e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10d0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10d0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10d0e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="10d0e-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10d0e-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="10d0e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10d0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10d0e-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10d0e-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="10d0e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10d0e-115">Application</span></span> | <span data-ttu-id="10d0e-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10d0e-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="10d0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10d0e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="10d0e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10d0e-118">Request headers</span></span>
| <span data-ttu-id="10d0e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10d0e-119">Header</span></span>       | <span data-ttu-id="10d0e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="10d0e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="10d0e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="10d0e-121">Authorization</span></span>  | <span data-ttu-id="10d0e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10d0e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="10d0e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10d0e-124">Content-Type</span></span>  | <span data-ttu-id="10d0e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10d0e-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="10d0e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10d0e-127">Request body</span></span>
<span data-ttu-id="10d0e-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="10d0e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="10d0e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10d0e-131">Property</span></span>     | <span data-ttu-id="10d0e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="10d0e-132">Type</span></span>   |<span data-ttu-id="10d0e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="10d0e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10d0e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="10d0e-134">displayName</span></span>|<span data-ttu-id="10d0e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10d0e-135">String</span></span>|<span data-ttu-id="10d0e-136">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="10d0e-136">The folder's display name.</span></span>|
|<span data-ttu-id="10d0e-137">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="10d0e-137">parentFolderId</span></span>|<span data-ttu-id="10d0e-138">String</span><span class="sxs-lookup"><span data-stu-id="10d0e-138">String</span></span>|<span data-ttu-id="10d0e-139">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="10d0e-139">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="10d0e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="10d0e-140">Response</span></span>

<span data-ttu-id="10d0e-141">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10d0e-141">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10d0e-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10d0e-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10d0e-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10d0e-143">Request</span></span>
<span data-ttu-id="10d0e-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10d0e-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10d0e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="10d0e-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="10d0e-146">C#</span><span class="sxs-lookup"><span data-stu-id="10d0e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10d0e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10d0e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10d0e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10d0e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10d0e-149">Java</span><span class="sxs-lookup"><span data-stu-id="10d0e-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="10d0e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="10d0e-150">Response</span></span>
<span data-ttu-id="10d0e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10d0e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
