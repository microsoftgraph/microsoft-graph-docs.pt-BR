---
title: Atualizar contactfolder
description: Atualiza as propriedades do objeto contactfolder.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 471b2965e39c8aa43e01f7df6bae1aaf91792b2e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047060"
---
# <a name="update-contactfolder"></a><span data-ttu-id="b7a99-103">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="b7a99-103">Update contactfolder</span></span>

<span data-ttu-id="b7a99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7a99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7a99-105">Atualiza as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="b7a99-105">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7a99-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7a99-106">Permissions</span></span>
<span data-ttu-id="b7a99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7a99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7a99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7a99-109">Permission type</span></span>      | <span data-ttu-id="b7a99-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7a99-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7a99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7a99-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7a99-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7a99-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b7a99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7a99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7a99-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7a99-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b7a99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7a99-115">Application</span></span> | <span data-ttu-id="b7a99-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7a99-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7a99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7a99-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b7a99-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a99-118">Request headers</span></span>
| <span data-ttu-id="b7a99-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7a99-119">Header</span></span>       | <span data-ttu-id="b7a99-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b7a99-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7a99-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7a99-121">Authorization</span></span>  | <span data-ttu-id="b7a99-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7a99-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b7a99-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7a99-124">Content-Type</span></span>  | <span data-ttu-id="b7a99-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7a99-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7a99-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a99-127">Request body</span></span>
<span data-ttu-id="b7a99-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b7a99-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b7a99-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7a99-131">Property</span></span>     | <span data-ttu-id="b7a99-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7a99-132">Type</span></span>   |<span data-ttu-id="b7a99-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7a99-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7a99-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b7a99-134">displayName</span></span>|<span data-ttu-id="b7a99-135">String</span><span class="sxs-lookup"><span data-stu-id="b7a99-135">String</span></span>|<span data-ttu-id="b7a99-136">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="b7a99-136">The folder's display name.</span></span>|
|<span data-ttu-id="b7a99-137">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b7a99-137">parentFolderId</span></span>|<span data-ttu-id="b7a99-138">String</span><span class="sxs-lookup"><span data-stu-id="b7a99-138">String</span></span>|<span data-ttu-id="b7a99-139">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="b7a99-139">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="b7a99-140">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="b7a99-140">wellKnownName</span></span>|<span data-ttu-id="b7a99-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7a99-141">string</span></span>|<span data-ttu-id="b7a99-142">O nome da pasta se a pasta for uma pasta reconhecida.</span><span class="sxs-lookup"><span data-stu-id="b7a99-142">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="b7a99-143">Atualmente é `contacts` a única pasta de contatos reconhecida.</span><span class="sxs-lookup"><span data-stu-id="b7a99-143">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="b7a99-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a99-144">Response</span></span>

<span data-ttu-id="b7a99-145">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7a99-145">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7a99-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7a99-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7a99-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a99-147">Request</span></span>
<span data-ttu-id="b7a99-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7a99-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7a99-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7a99-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b7a99-150">C#</span><span class="sxs-lookup"><span data-stu-id="b7a99-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7a99-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7a99-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7a99-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7a99-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7a99-153">Java</span><span class="sxs-lookup"><span data-stu-id="b7a99-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b7a99-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a99-154">Response</span></span>
<span data-ttu-id="b7a99-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7a99-155">Here is an example of the response.</span></span> <span data-ttu-id="b7a99-156">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b7a99-156">Note: The response object shown here might be shortened for readability.</span></span>
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
  "wellKnownName": "wellKnownName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


