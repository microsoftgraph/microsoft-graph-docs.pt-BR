---
title: 'página: copyToSection'
description: Copia uma página para uma seção específica.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 5811772360cfd6c50a75d664396de6638078b31b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596176"
---
# <a name="page-copytosection"></a><span data-ttu-id="a86b5-103">página: copyToSection</span><span class="sxs-lookup"><span data-stu-id="a86b5-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a86b5-104">Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="a86b5-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="a86b5-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="a86b5-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="a86b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a86b5-106">Permissions</span></span>
<span data-ttu-id="a86b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a86b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a86b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a86b5-109">Permission type</span></span>      | <span data-ttu-id="a86b5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a86b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a86b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a86b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a86b5-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a86b5-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a86b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a86b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a86b5-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a86b5-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a86b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a86b5-115">Application</span></span> | <span data-ttu-id="a86b5-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a86b5-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a86b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a86b5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="a86b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a86b5-118">Request headers</span></span>
| <span data-ttu-id="a86b5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a86b5-119">Name</span></span>       | <span data-ttu-id="a86b5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a86b5-120">Type</span></span> | <span data-ttu-id="a86b5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a86b5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a86b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a86b5-122">Authorization</span></span>  | <span data-ttu-id="a86b5-123">string</span><span class="sxs-lookup"><span data-stu-id="a86b5-123">string</span></span>  | <span data-ttu-id="a86b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a86b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a86b5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a86b5-126">Content-Type</span></span> | <span data-ttu-id="a86b5-127">string</span><span class="sxs-lookup"><span data-stu-id="a86b5-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a86b5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a86b5-128">Request body</span></span>
<span data-ttu-id="a86b5-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="a86b5-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="a86b5-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a86b5-130">Parameter</span></span>    | <span data-ttu-id="a86b5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a86b5-131">Type</span></span>   |<span data-ttu-id="a86b5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a86b5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a86b5-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="a86b5-133">siteCollectionId</span></span>|<span data-ttu-id="a86b5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a86b5-134">String</span></span>|<span data-ttu-id="a86b5-135">A ID do site do SharePoint para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="a86b5-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="a86b5-136">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a86b5-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="a86b5-137">siteId</span><span class="sxs-lookup"><span data-stu-id="a86b5-137">siteId</span></span>|<span data-ttu-id="a86b5-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a86b5-138">String</span></span>|<span data-ttu-id="a86b5-139">A ID da Web do SharePoint a ser copiada.</span><span class="sxs-lookup"><span data-stu-id="a86b5-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="a86b5-140">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a86b5-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="a86b5-141">groupId</span><span class="sxs-lookup"><span data-stu-id="a86b5-141">groupId</span></span>|<span data-ttu-id="a86b5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a86b5-142">String</span></span>|<span data-ttu-id="a86b5-143">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="a86b5-143">The id of the group to copy to.</span></span> <span data-ttu-id="a86b5-144">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a86b5-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="a86b5-145">id</span><span class="sxs-lookup"><span data-stu-id="a86b5-145">id</span></span>|<span data-ttu-id="a86b5-146">String</span><span class="sxs-lookup"><span data-stu-id="a86b5-146">String</span></span>|<span data-ttu-id="a86b5-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a86b5-147">Required.</span></span> <span data-ttu-id="a86b5-148">A ID da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="a86b5-148">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="a86b5-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a86b5-149">Response</span></span>

<span data-ttu-id="a86b5-150">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="a86b5-150">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="a86b5-151">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="a86b5-151">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="a86b5-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a86b5-152">Example</span></span>
<span data-ttu-id="a86b5-153">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a86b5-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a86b5-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a86b5-154">Request</span></span>
<span data-ttu-id="a86b5-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a86b5-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a86b5-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a86b5-156">Response</span></span>
<span data-ttu-id="a86b5-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a86b5-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a86b5-158">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a86b5-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a86b5-159">Basic</span><span class="sxs-lookup"><span data-stu-id="a86b5-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/page_copytosection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a86b5-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a86b5-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/page_copytosection-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
