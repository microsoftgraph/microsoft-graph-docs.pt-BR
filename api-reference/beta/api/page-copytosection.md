---
title: 'página: copyToSection'
description: Copia uma página para uma seção específica.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 2f37685212c48f3afe75a9c7daf2776f08aa92f6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896431"
---
# <a name="page-copytosection"></a><span data-ttu-id="e3722-103">página: copyToSection</span><span class="sxs-lookup"><span data-stu-id="e3722-103">page: copyToSection</span></span>

<span data-ttu-id="e3722-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3722-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3722-105">Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="e3722-105">Copies a page to a specific section.</span></span>

<span data-ttu-id="e3722-106">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="e3722-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3722-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3722-107">Permissions</span></span>
<span data-ttu-id="e3722-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e3722-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e3722-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3722-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3722-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3722-110">Permission type</span></span>      | <span data-ttu-id="e3722-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3722-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3722-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3722-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3722-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3722-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3722-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3722-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3722-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3722-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e3722-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3722-116">Application</span></span> | <span data-ttu-id="e3722-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3722-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3722-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3722-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="e3722-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3722-119">Request headers</span></span>
| <span data-ttu-id="e3722-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e3722-120">Name</span></span>       | <span data-ttu-id="e3722-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3722-121">Type</span></span> | <span data-ttu-id="e3722-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3722-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e3722-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3722-123">Authorization</span></span>  | <span data-ttu-id="e3722-124">string</span><span class="sxs-lookup"><span data-stu-id="e3722-124">string</span></span>  | <span data-ttu-id="e3722-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e3722-125">Bearer {token}.</span></span> <span data-ttu-id="e3722-126">Required.</span><span class="sxs-lookup"><span data-stu-id="e3722-126">Required.</span></span> |
| <span data-ttu-id="e3722-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3722-127">Content-Type</span></span> | <span data-ttu-id="e3722-128">string</span><span class="sxs-lookup"><span data-stu-id="e3722-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e3722-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3722-129">Request body</span></span>
<span data-ttu-id="e3722-130">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="e3722-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="e3722-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e3722-131">Parameter</span></span>    | <span data-ttu-id="e3722-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3722-132">Type</span></span>   |<span data-ttu-id="e3722-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3722-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3722-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="e3722-134">siteCollectionId</span></span>|<span data-ttu-id="e3722-135">String</span><span class="sxs-lookup"><span data-stu-id="e3722-135">String</span></span>|<span data-ttu-id="e3722-136">A ID do site do SharePoint para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="e3722-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="e3722-137">Use somente ao copiar para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e3722-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="e3722-138">siteId</span><span class="sxs-lookup"><span data-stu-id="e3722-138">siteId</span></span>|<span data-ttu-id="e3722-139">String</span><span class="sxs-lookup"><span data-stu-id="e3722-139">String</span></span>|<span data-ttu-id="e3722-140">A ID da Web do SharePoint a ser copiada.</span><span class="sxs-lookup"><span data-stu-id="e3722-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="e3722-141">Use somente ao copiar para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e3722-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="e3722-142">groupId</span><span class="sxs-lookup"><span data-stu-id="e3722-142">groupId</span></span>|<span data-ttu-id="e3722-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3722-143">String</span></span>|<span data-ttu-id="e3722-144">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="e3722-144">The id of the group to copy to.</span></span> <span data-ttu-id="e3722-145">Use somente ao copiar para um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e3722-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="e3722-146">id</span><span class="sxs-lookup"><span data-stu-id="e3722-146">id</span></span>|<span data-ttu-id="e3722-147">String</span><span class="sxs-lookup"><span data-stu-id="e3722-147">String</span></span>|<span data-ttu-id="e3722-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3722-148">Required.</span></span> <span data-ttu-id="e3722-149">A ID da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="e3722-149">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="e3722-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3722-150">Response</span></span>

<span data-ttu-id="e3722-151">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um `Operation-Location` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="e3722-151">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="e3722-152">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="e3722-152">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="e3722-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3722-153">Example</span></span>
<span data-ttu-id="e3722-154">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e3722-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e3722-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3722-155">Request</span></span>
<span data-ttu-id="e3722-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3722-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3722-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3722-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e3722-158">C#</span><span class="sxs-lookup"><span data-stu-id="e3722-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3722-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3722-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3722-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3722-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3722-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3722-161">Response</span></span>
<span data-ttu-id="e3722-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3722-162">Here is an example of the response.</span></span>
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
