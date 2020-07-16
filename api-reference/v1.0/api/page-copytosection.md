---
title: 'página: copyToSection'
description: Copia uma página para uma seção específica.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 245f5b760d4a755162107267b1836c5760a1c22a
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898335"
---
# <a name="page-copytosection"></a><span data-ttu-id="861da-103">página: copyToSection</span><span class="sxs-lookup"><span data-stu-id="861da-103">page: copyToSection</span></span>

<span data-ttu-id="861da-104">Namespace: Microsoft. Graph copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="861da-104">Namespace: microsoft.graph Copies a page to a specific section.</span></span>

<span data-ttu-id="861da-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="861da-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="861da-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="861da-106">Permissions</span></span>
<span data-ttu-id="861da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="861da-109">Permission type</span></span>      | <span data-ttu-id="861da-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="861da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="861da-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="861da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="861da-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861da-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="861da-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="861da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="861da-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="861da-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="861da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="861da-115">Application</span></span> | <span data-ttu-id="861da-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861da-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="861da-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="861da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="861da-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="861da-118">Request headers</span></span>
| <span data-ttu-id="861da-119">Nome</span><span class="sxs-lookup"><span data-stu-id="861da-119">Name</span></span>       | <span data-ttu-id="861da-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="861da-120">Type</span></span> | <span data-ttu-id="861da-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="861da-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="861da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="861da-122">Authorization</span></span>  | <span data-ttu-id="861da-123">string</span><span class="sxs-lookup"><span data-stu-id="861da-123">string</span></span>  | <span data-ttu-id="861da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="861da-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="861da-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="861da-126">Content-Type</span></span> | <span data-ttu-id="861da-127">string</span><span class="sxs-lookup"><span data-stu-id="861da-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="861da-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="861da-128">Request body</span></span>
<span data-ttu-id="861da-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="861da-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="861da-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="861da-130">Parameter</span></span>    | <span data-ttu-id="861da-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="861da-131">Type</span></span>   |<span data-ttu-id="861da-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="861da-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="861da-133">groupId</span><span class="sxs-lookup"><span data-stu-id="861da-133">groupId</span></span>|<span data-ttu-id="861da-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861da-134">String</span></span>|<span data-ttu-id="861da-135">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="861da-135">The id of the group to copy to.</span></span> <span data-ttu-id="861da-136">Use somente ao copiar para um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="861da-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="861da-137">id</span><span class="sxs-lookup"><span data-stu-id="861da-137">id</span></span>|<span data-ttu-id="861da-138">String</span><span class="sxs-lookup"><span data-stu-id="861da-138">String</span></span>|<span data-ttu-id="861da-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="861da-139">Required.</span></span> <span data-ttu-id="861da-140">A ID da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="861da-140">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="861da-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="861da-141">Response</span></span>

<span data-ttu-id="861da-142">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um `Operation-Location` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="861da-142">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="861da-143">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="861da-143">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="861da-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="861da-144">Example</span></span>
<span data-ttu-id="861da-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="861da-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="861da-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="861da-146">Request</span></span>
<span data-ttu-id="861da-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="861da-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="861da-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="861da-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="861da-149">C#</span><span class="sxs-lookup"><span data-stu-id="861da-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="861da-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="861da-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="861da-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="861da-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="861da-152">Java</span><span class="sxs-lookup"><span data-stu-id="861da-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="861da-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="861da-153">Response</span></span>
<span data-ttu-id="861da-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="861da-154">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
