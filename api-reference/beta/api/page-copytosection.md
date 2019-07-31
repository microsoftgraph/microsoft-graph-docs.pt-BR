---
title: 'página: copyToSection'
description: Copia uma página para uma seção específica.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: fe8e0a18e91ecdad9daa648eb8a9944cad7a14de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992420"
---
# <a name="page-copytosection"></a><span data-ttu-id="2bdc6-103">página: copyToSection</span><span class="sxs-lookup"><span data-stu-id="2bdc6-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bdc6-104">Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="2bdc6-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bdc6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2bdc6-106">Permissions</span></span>
<span data-ttu-id="2bdc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bdc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bdc6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bdc6-109">Permission type</span></span>      | <span data-ttu-id="2bdc6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2bdc6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bdc6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bdc6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2bdc6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bdc6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2bdc6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bdc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bdc6-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2bdc6-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2bdc6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bdc6-115">Application</span></span> | <span data-ttu-id="2bdc6-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bdc6-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bdc6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bdc6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="2bdc6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdc6-118">Request headers</span></span>
| <span data-ttu-id="2bdc6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2bdc6-119">Name</span></span>       | <span data-ttu-id="2bdc6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bdc6-120">Type</span></span> | <span data-ttu-id="2bdc6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bdc6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2bdc6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bdc6-122">Authorization</span></span>  | <span data-ttu-id="2bdc6-123">string</span><span class="sxs-lookup"><span data-stu-id="2bdc6-123">string</span></span>  | <span data-ttu-id="2bdc6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2bdc6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2bdc6-126">Content-Type</span></span> | <span data-ttu-id="2bdc6-127">string</span><span class="sxs-lookup"><span data-stu-id="2bdc6-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="2bdc6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdc6-128">Request body</span></span>
<span data-ttu-id="2bdc6-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="2bdc6-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2bdc6-130">Parameter</span></span>    | <span data-ttu-id="2bdc6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bdc6-131">Type</span></span>   |<span data-ttu-id="2bdc6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bdc6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bdc6-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="2bdc6-133">siteCollectionId</span></span>|<span data-ttu-id="2bdc6-134">String</span><span class="sxs-lookup"><span data-stu-id="2bdc6-134">String</span></span>|<span data-ttu-id="2bdc6-135">A ID do site do SharePoint para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="2bdc6-136">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="2bdc6-137">siteId</span><span class="sxs-lookup"><span data-stu-id="2bdc6-137">siteId</span></span>|<span data-ttu-id="2bdc6-138">String</span><span class="sxs-lookup"><span data-stu-id="2bdc6-138">String</span></span>|<span data-ttu-id="2bdc6-139">A ID da Web do SharePoint a ser copiada.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="2bdc6-140">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="2bdc6-141">groupId</span><span class="sxs-lookup"><span data-stu-id="2bdc6-141">groupId</span></span>|<span data-ttu-id="2bdc6-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bdc6-142">String</span></span>|<span data-ttu-id="2bdc6-143">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-143">The id of the group to copy to.</span></span> <span data-ttu-id="2bdc6-144">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="2bdc6-145">id</span><span class="sxs-lookup"><span data-stu-id="2bdc6-145">id</span></span>|<span data-ttu-id="2bdc6-146">String</span><span class="sxs-lookup"><span data-stu-id="2bdc6-146">String</span></span>|<span data-ttu-id="2bdc6-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-147">Required.</span></span> <span data-ttu-id="2bdc6-148">A ID da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-148">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="2bdc6-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdc6-149">Response</span></span>

<span data-ttu-id="2bdc6-150">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-150">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="2bdc6-151">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="2bdc6-151">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="2bdc6-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bdc6-152">Example</span></span>
<span data-ttu-id="2bdc6-153">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2bdc6-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdc6-154">Request</span></span>
<span data-ttu-id="2bdc6-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-155">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2bdc6-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bdc6-156">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2bdc6-157">C#</span><span class="sxs-lookup"><span data-stu-id="2bdc6-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2bdc6-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="2bdc6-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2bdc6-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2bdc6-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2bdc6-160">Java</span><span class="sxs-lookup"><span data-stu-id="2bdc6-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2bdc6-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdc6-161">Response</span></span>
<span data-ttu-id="2bdc6-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bdc6-162">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
