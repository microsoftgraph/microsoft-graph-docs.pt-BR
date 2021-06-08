---
title: 'bloco de anotações: copyNotebook'
description: Copia um bloco de anotações para a pasta Blocos de Anotações na biblioteca de documentos de destino. A pasta será criada se ela não existir.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 6f22838e9af2103f83f2c065e1376f931152fc2e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786128"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="d8c4b-104">bloco de anotações: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="d8c4b-104">notebook: copyNotebook</span></span>

<span data-ttu-id="d8c4b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8c4b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8c4b-106">Copia um bloco de anotações para a pasta Blocos de Anotações na biblioteca de documentos de destino.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-106">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="d8c4b-107">A pasta será criada se ela não existir.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-107">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="d8c4b-108">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro chame a ação Copiar e, em seguida, sonda o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-108">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8c4b-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="d8c4b-109">Permissions</span></span>
<span data-ttu-id="d8c4b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8c4b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8c4b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8c4b-112">Permission type</span></span>      | <span data-ttu-id="d8c4b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8c4b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8c4b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8c4b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d8c4b-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8c4b-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8c4b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8c4b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8c4b-117">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c4b-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d8c4b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8c4b-118">Application</span></span> | <span data-ttu-id="d8c4b-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8c4b-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8c4b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8c4b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="d8c4b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8c4b-121">Request headers</span></span>
| <span data-ttu-id="d8c4b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d8c4b-122">Name</span></span>       | <span data-ttu-id="d8c4b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8c4b-123">Type</span></span> | <span data-ttu-id="d8c4b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8c4b-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d8c4b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8c4b-125">Authorization</span></span>  | <span data-ttu-id="d8c4b-126">string</span><span class="sxs-lookup"><span data-stu-id="d8c4b-126">string</span></span>  | <span data-ttu-id="d8c4b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8c4b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8c4b-129">Content-Type</span></span> | <span data-ttu-id="d8c4b-130">string</span><span class="sxs-lookup"><span data-stu-id="d8c4b-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d8c4b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8c4b-131">Request body</span></span>
<span data-ttu-id="d8c4b-132">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-132">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="d8c4b-133">Não há problema em enviar um corpo vazio se nenhum for necessário.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-133">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="d8c4b-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d8c4b-134">Parameter</span></span>    | <span data-ttu-id="d8c4b-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8c4b-135">Type</span></span>   |<span data-ttu-id="d8c4b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8c4b-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8c4b-137">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="d8c4b-137">siteCollectionId</span></span>|<span data-ttu-id="d8c4b-138">String</span><span class="sxs-lookup"><span data-stu-id="d8c4b-138">String</span></span>|<span data-ttu-id="d8c4b-139">A id do site SharePoint para o que copiar.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-139">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="d8c4b-140">Use somente ao copiar para um SharePoint site.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-140">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="d8c4b-141">siteId</span><span class="sxs-lookup"><span data-stu-id="d8c4b-141">siteId</span></span>|<span data-ttu-id="d8c4b-142">String</span><span class="sxs-lookup"><span data-stu-id="d8c4b-142">String</span></span>|<span data-ttu-id="d8c4b-143">A id do SharePoint web para o que copiar.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-143">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="d8c4b-144">Use somente ao copiar para um SharePoint site.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-144">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="d8c4b-145">groupId</span><span class="sxs-lookup"><span data-stu-id="d8c4b-145">groupId</span></span>|<span data-ttu-id="d8c4b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8c4b-146">String</span></span>|<span data-ttu-id="d8c4b-147">A id do grupo para o que copiar.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-147">The id of the group to copy to.</span></span> <span data-ttu-id="d8c4b-148">Use somente ao copiar para um Microsoft 365 grupo.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-148">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="d8c4b-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="d8c4b-149">renameAs</span></span>|<span data-ttu-id="d8c4b-150">String</span><span class="sxs-lookup"><span data-stu-id="d8c4b-150">String</span></span>|<span data-ttu-id="d8c4b-151">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-151">The name of the copy.</span></span> <span data-ttu-id="d8c4b-152">Padrão para o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="d8c4b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8c4b-153">Response</span></span>

<span data-ttu-id="d8c4b-154">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e um `Operation-Location` header.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="d8c4b-155">Sondar Operation-Location ponto de extremidade para [obter o status da operação de cópia.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="d8c4b-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="d8c4b-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8c4b-156">Example</span></span>
<span data-ttu-id="d8c4b-157">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d8c4b-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8c4b-158">Request</span></span>
<span data-ttu-id="d8c4b-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8c4b-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8c4b-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d8c4b-161">C#</span><span class="sxs-lookup"><span data-stu-id="d8c4b-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8c4b-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8c4b-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8c4b-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8c4b-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8c4b-164">Java</span><span class="sxs-lookup"><span data-stu-id="d8c4b-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8c4b-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8c4b-165">Response</span></span>
<span data-ttu-id="d8c4b-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8c4b-166">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


