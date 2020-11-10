---
title: 'seção: copyToNotebook'
description: Copia uma seção para um bloco de anotações específico.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5a1d99f93df7acd6c964ae690784ab3df8cca43c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978680"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="88b65-103">seção: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="88b65-103">section: copyToNotebook</span></span>

<span data-ttu-id="88b65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88b65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88b65-105">Copia uma seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="88b65-105">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="88b65-106">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="88b65-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="88b65-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="88b65-107">Permissions</span></span>
<span data-ttu-id="88b65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88b65-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88b65-110">Permission type</span></span>      | <span data-ttu-id="88b65-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88b65-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88b65-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88b65-112">Delegated (work or school account)</span></span> | <span data-ttu-id="88b65-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88b65-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="88b65-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88b65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88b65-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88b65-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="88b65-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88b65-116">Application</span></span> | <span data-ttu-id="88b65-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88b65-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88b65-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88b65-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="88b65-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88b65-119">Request headers</span></span>
| <span data-ttu-id="88b65-120">Nome</span><span class="sxs-lookup"><span data-stu-id="88b65-120">Name</span></span>       | <span data-ttu-id="88b65-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="88b65-121">Type</span></span> | <span data-ttu-id="88b65-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="88b65-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="88b65-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88b65-123">Authorization</span></span>  | <span data-ttu-id="88b65-124">string</span><span class="sxs-lookup"><span data-stu-id="88b65-124">string</span></span>  | <span data-ttu-id="88b65-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88b65-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88b65-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88b65-127">Content-Type</span></span> | <span data-ttu-id="88b65-128">string</span><span class="sxs-lookup"><span data-stu-id="88b65-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="88b65-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88b65-129">Request body</span></span>
<span data-ttu-id="88b65-130">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="88b65-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="88b65-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="88b65-131">Parameter</span></span>    | <span data-ttu-id="88b65-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="88b65-132">Type</span></span>   |<span data-ttu-id="88b65-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="88b65-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88b65-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="88b65-134">siteCollectionId</span></span>|<span data-ttu-id="88b65-135">String</span><span class="sxs-lookup"><span data-stu-id="88b65-135">String</span></span>|<span data-ttu-id="88b65-136">A ID do site do SharePoint para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="88b65-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="88b65-137">Use somente ao copiar para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="88b65-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="88b65-138">siteId</span><span class="sxs-lookup"><span data-stu-id="88b65-138">siteId</span></span>|<span data-ttu-id="88b65-139">String</span><span class="sxs-lookup"><span data-stu-id="88b65-139">String</span></span>|<span data-ttu-id="88b65-140">A ID da Web do SharePoint a ser copiada.</span><span class="sxs-lookup"><span data-stu-id="88b65-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="88b65-141">Use somente ao copiar para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="88b65-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="88b65-142">groupId</span><span class="sxs-lookup"><span data-stu-id="88b65-142">groupId</span></span>|<span data-ttu-id="88b65-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88b65-143">String</span></span>|<span data-ttu-id="88b65-144">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="88b65-144">The id of the group to copy to.</span></span> <span data-ttu-id="88b65-145">Use somente ao copiar para um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="88b65-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="88b65-146">id</span><span class="sxs-lookup"><span data-stu-id="88b65-146">id</span></span>|<span data-ttu-id="88b65-147">String</span><span class="sxs-lookup"><span data-stu-id="88b65-147">String</span></span>|<span data-ttu-id="88b65-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88b65-148">Required.</span></span> <span data-ttu-id="88b65-149">A ID do bloco de anotações de destino.</span><span class="sxs-lookup"><span data-stu-id="88b65-149">The id of the destination notebook.</span></span> |
|<span data-ttu-id="88b65-150">renomeas</span><span class="sxs-lookup"><span data-stu-id="88b65-150">renameAs</span></span>|<span data-ttu-id="88b65-151">String</span><span class="sxs-lookup"><span data-stu-id="88b65-151">String</span></span>|<span data-ttu-id="88b65-152">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="88b65-152">The name of the copy.</span></span> <span data-ttu-id="88b65-153">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="88b65-153">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="88b65-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="88b65-154">Response</span></span>

<span data-ttu-id="88b65-155">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um `Operation-Location` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="88b65-155">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="88b65-156">Sondar o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="88b65-156">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="88b65-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88b65-157">Example</span></span>
<span data-ttu-id="88b65-158">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="88b65-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="88b65-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88b65-159">Request</span></span>
<span data-ttu-id="88b65-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88b65-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88b65-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="88b65-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="88b65-162">C#</span><span class="sxs-lookup"><span data-stu-id="88b65-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88b65-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88b65-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88b65-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88b65-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88b65-165">Java</span><span class="sxs-lookup"><span data-stu-id="88b65-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytonotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="88b65-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="88b65-166">Response</span></span>
<span data-ttu-id="88b65-167">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88b65-167">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


