---
title: 'page: copyToSection'
description: Copia uma página para uma seção específica.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 665d244248c8af3a4ce3b5b01151d3debe196d92
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785232"
---
# <a name="page-copytosection"></a><span data-ttu-id="1ff95-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="1ff95-103">page: copyToSection</span></span>

<span data-ttu-id="1ff95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ff95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ff95-105">Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="1ff95-105">Copies a page to a specific section.</span></span>

<span data-ttu-id="1ff95-106">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro chame a ação Copiar e, em seguida, sonda o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="1ff95-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ff95-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1ff95-107">Permissions</span></span>
<span data-ttu-id="1ff95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ff95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ff95-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ff95-110">Permission type</span></span>      | <span data-ttu-id="1ff95-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ff95-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ff95-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ff95-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1ff95-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ff95-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ff95-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ff95-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ff95-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ff95-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1ff95-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ff95-116">Application</span></span> | <span data-ttu-id="1ff95-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ff95-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ff95-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff95-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="1ff95-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff95-119">Request headers</span></span>
| <span data-ttu-id="1ff95-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1ff95-120">Name</span></span>       | <span data-ttu-id="1ff95-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ff95-121">Type</span></span> | <span data-ttu-id="1ff95-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ff95-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1ff95-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ff95-123">Authorization</span></span>  | <span data-ttu-id="1ff95-124">string</span><span class="sxs-lookup"><span data-stu-id="1ff95-124">string</span></span>  | <span data-ttu-id="1ff95-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ff95-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ff95-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ff95-127">Content-Type</span></span> | <span data-ttu-id="1ff95-128">string</span><span class="sxs-lookup"><span data-stu-id="1ff95-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1ff95-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff95-129">Request body</span></span>
<span data-ttu-id="1ff95-130">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="1ff95-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="1ff95-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1ff95-131">Parameter</span></span>    | <span data-ttu-id="1ff95-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ff95-132">Type</span></span>   |<span data-ttu-id="1ff95-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ff95-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ff95-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="1ff95-134">siteCollectionId</span></span>|<span data-ttu-id="1ff95-135">String</span><span class="sxs-lookup"><span data-stu-id="1ff95-135">String</span></span>|<span data-ttu-id="1ff95-136">A id do site SharePoint para o que copiar.</span><span class="sxs-lookup"><span data-stu-id="1ff95-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="1ff95-137">Use somente ao copiar para um SharePoint site.</span><span class="sxs-lookup"><span data-stu-id="1ff95-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="1ff95-138">siteId</span><span class="sxs-lookup"><span data-stu-id="1ff95-138">siteId</span></span>|<span data-ttu-id="1ff95-139">String</span><span class="sxs-lookup"><span data-stu-id="1ff95-139">String</span></span>|<span data-ttu-id="1ff95-140">A id do SharePoint web para o que copiar.</span><span class="sxs-lookup"><span data-stu-id="1ff95-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="1ff95-141">Use somente ao copiar para um SharePoint site.</span><span class="sxs-lookup"><span data-stu-id="1ff95-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="1ff95-142">groupId</span><span class="sxs-lookup"><span data-stu-id="1ff95-142">groupId</span></span>|<span data-ttu-id="1ff95-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ff95-143">String</span></span>|<span data-ttu-id="1ff95-144">A id do grupo para o que copiar.</span><span class="sxs-lookup"><span data-stu-id="1ff95-144">The id of the group to copy to.</span></span> <span data-ttu-id="1ff95-145">Use somente ao copiar para um Microsoft 365 grupo.</span><span class="sxs-lookup"><span data-stu-id="1ff95-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="1ff95-146">id</span><span class="sxs-lookup"><span data-stu-id="1ff95-146">id</span></span>|<span data-ttu-id="1ff95-147">String</span><span class="sxs-lookup"><span data-stu-id="1ff95-147">String</span></span>|<span data-ttu-id="1ff95-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ff95-148">Required.</span></span> <span data-ttu-id="1ff95-149">A id da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="1ff95-149">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="1ff95-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff95-150">Response</span></span>

<span data-ttu-id="1ff95-151">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e um `Operation-Location` header.</span><span class="sxs-lookup"><span data-stu-id="1ff95-151">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="1ff95-152">Sondar Operation-Location ponto de extremidade para [obter o status da operação de cópia.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="1ff95-152">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="1ff95-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ff95-153">Example</span></span>
<span data-ttu-id="1ff95-154">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1ff95-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1ff95-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff95-155">Request</span></span>
<span data-ttu-id="1ff95-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ff95-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ff95-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff95-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1ff95-158">C#</span><span class="sxs-lookup"><span data-stu-id="1ff95-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ff95-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ff95-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ff95-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ff95-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ff95-161">Java</span><span class="sxs-lookup"><span data-stu-id="1ff95-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1ff95-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff95-162">Response</span></span>
<span data-ttu-id="1ff95-163">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ff95-163">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


