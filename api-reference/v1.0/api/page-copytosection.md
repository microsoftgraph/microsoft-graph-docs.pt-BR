---
title: 'page: copyToSection'
description: Copia uma página para uma seção específica.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c9bdd57eaa929c47ed6dfe5429086e0f78760e06
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788063"
---
# <a name="page-copytosection"></a><span data-ttu-id="d3dd9-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="d3dd9-103">page: copyToSection</span></span>

<span data-ttu-id="d3dd9-104">Namespace: microsoft.graph Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-104">Namespace: microsoft.graph Copies a page to a specific section.</span></span>

<span data-ttu-id="d3dd9-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro chame a ação Copiar e, em seguida, sonda o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3dd9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3dd9-106">Permissions</span></span>
<span data-ttu-id="d3dd9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3dd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3dd9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3dd9-109">Permission type</span></span>      | <span data-ttu-id="d3dd9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3dd9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3dd9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3dd9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3dd9-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3dd9-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3dd9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3dd9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3dd9-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3dd9-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d3dd9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3dd9-115">Application</span></span> | <span data-ttu-id="d3dd9-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3dd9-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3dd9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3dd9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="d3dd9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3dd9-118">Request headers</span></span>
| <span data-ttu-id="d3dd9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d3dd9-119">Name</span></span>       | <span data-ttu-id="d3dd9-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3dd9-120">Type</span></span> | <span data-ttu-id="d3dd9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3dd9-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d3dd9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3dd9-122">Authorization</span></span>  | <span data-ttu-id="d3dd9-123">string</span><span class="sxs-lookup"><span data-stu-id="d3dd9-123">string</span></span>  | <span data-ttu-id="d3dd9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3dd9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3dd9-126">Content-Type</span></span> | <span data-ttu-id="d3dd9-127">string</span><span class="sxs-lookup"><span data-stu-id="d3dd9-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d3dd9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3dd9-128">Request body</span></span>
<span data-ttu-id="d3dd9-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="d3dd9-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d3dd9-130">Parameter</span></span>    | <span data-ttu-id="d3dd9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3dd9-131">Type</span></span>   |<span data-ttu-id="d3dd9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3dd9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3dd9-133">groupId</span><span class="sxs-lookup"><span data-stu-id="d3dd9-133">groupId</span></span>|<span data-ttu-id="d3dd9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3dd9-134">String</span></span>|<span data-ttu-id="d3dd9-135">A id do grupo para o que copiar.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-135">The id of the group to copy to.</span></span> <span data-ttu-id="d3dd9-136">Use somente ao copiar para um Microsoft 365 grupo.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="d3dd9-137">id</span><span class="sxs-lookup"><span data-stu-id="d3dd9-137">id</span></span>|<span data-ttu-id="d3dd9-138">String</span><span class="sxs-lookup"><span data-stu-id="d3dd9-138">String</span></span>|<span data-ttu-id="d3dd9-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-139">Required.</span></span> <span data-ttu-id="d3dd9-140">A id da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-140">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="d3dd9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3dd9-141">Response</span></span>

<span data-ttu-id="d3dd9-142">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e um `Operation-Location` header.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-142">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="d3dd9-143">Sondar Operation-Location ponto de extremidade para [obter o status da operação de cópia.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="d3dd9-143">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="d3dd9-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3dd9-144">Example</span></span>
<span data-ttu-id="d3dd9-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d3dd9-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3dd9-146">Request</span></span>
<span data-ttu-id="d3dd9-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3dd9-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3dd9-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d3dd9-149">C#</span><span class="sxs-lookup"><span data-stu-id="d3dd9-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3dd9-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3dd9-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3dd9-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3dd9-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3dd9-152">Java</span><span class="sxs-lookup"><span data-stu-id="d3dd9-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d3dd9-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3dd9-153">Response</span></span>
<span data-ttu-id="d3dd9-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3dd9-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

