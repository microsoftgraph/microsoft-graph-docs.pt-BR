---
title: 'seção: copyToNotebook'
description: Copia uma seção para um bloco de anotações específico.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f1a69334b10499295649ba09d64b1fa10bcb86b0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884398"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="31c57-103">seção: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="31c57-103">section: copyToNotebook</span></span>
<span data-ttu-id="31c57-104">Copia uma seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="31c57-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="31c57-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="31c57-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="31c57-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31c57-106">Permissions</span></span>
<span data-ttu-id="31c57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31c57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31c57-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31c57-109">Permission type</span></span>      | <span data-ttu-id="31c57-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31c57-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31c57-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31c57-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31c57-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c57-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="31c57-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31c57-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31c57-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31c57-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="31c57-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31c57-115">Application</span></span> | <span data-ttu-id="31c57-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c57-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31c57-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31c57-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="31c57-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31c57-118">Request headers</span></span>
| <span data-ttu-id="31c57-119">Nome</span><span class="sxs-lookup"><span data-stu-id="31c57-119">Name</span></span>       | <span data-ttu-id="31c57-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="31c57-120">Type</span></span> | <span data-ttu-id="31c57-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="31c57-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="31c57-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="31c57-122">Authorization</span></span>  | <span data-ttu-id="31c57-123">string</span><span class="sxs-lookup"><span data-stu-id="31c57-123">string</span></span>  | <span data-ttu-id="31c57-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31c57-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31c57-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31c57-126">Content-Type</span></span> | <span data-ttu-id="31c57-127">string</span><span class="sxs-lookup"><span data-stu-id="31c57-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="31c57-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31c57-128">Request body</span></span>
<span data-ttu-id="31c57-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="31c57-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="31c57-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="31c57-130">Parameter</span></span>    | <span data-ttu-id="31c57-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="31c57-131">Type</span></span>   |<span data-ttu-id="31c57-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="31c57-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31c57-133">groupId</span><span class="sxs-lookup"><span data-stu-id="31c57-133">groupId</span></span>|<span data-ttu-id="31c57-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31c57-134">String</span></span>|<span data-ttu-id="31c57-135">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="31c57-135">The id of the group to copy to.</span></span> <span data-ttu-id="31c57-136">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="31c57-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="31c57-137">id</span><span class="sxs-lookup"><span data-stu-id="31c57-137">id</span></span>|<span data-ttu-id="31c57-138">String</span><span class="sxs-lookup"><span data-stu-id="31c57-138">String</span></span>|<span data-ttu-id="31c57-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31c57-139">Required.</span></span> <span data-ttu-id="31c57-140">A ID do bloco de anotações de destino.</span><span class="sxs-lookup"><span data-stu-id="31c57-140">The id of the destination notebook.</span></span> |
|<span data-ttu-id="31c57-141">renomeas</span><span class="sxs-lookup"><span data-stu-id="31c57-141">renameAs</span></span>|<span data-ttu-id="31c57-142">String</span><span class="sxs-lookup"><span data-stu-id="31c57-142">String</span></span>|<span data-ttu-id="31c57-143">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="31c57-143">The name of the copy.</span></span> <span data-ttu-id="31c57-144">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="31c57-144">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="31c57-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="31c57-145">Response</span></span>

<span data-ttu-id="31c57-146">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="31c57-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="31c57-147">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="31c57-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="31c57-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31c57-148">Example</span></span>
<span data-ttu-id="31c57-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="31c57-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="31c57-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31c57-150">Request</span></span>
<span data-ttu-id="31c57-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31c57-151">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="31c57-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="31c57-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="31c57-153">C#</span><span class="sxs-lookup"><span data-stu-id="31c57-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31c57-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="31c57-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="31c57-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="31c57-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="31c57-156">Java</span><span class="sxs-lookup"><span data-stu-id="31c57-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytonotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="31c57-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="31c57-157">Response</span></span>
<span data-ttu-id="31c57-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31c57-158">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
