---
title: 'seção: copyToSectionGroup'
description: Copia uma seção para um grupo de seção específico.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: dc5ad2f046d13bde7d562d5221174cc9138a4b9e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896564"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="bb2d4-103">seção: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="bb2d4-103">section: copyToSectionGroup</span></span>

<span data-ttu-id="bb2d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb2d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb2d4-105">Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-105">Copies a section to a specific section group.</span></span>

<span data-ttu-id="bb2d4-106">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb2d4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb2d4-107">Permissions</span></span>
<span data-ttu-id="bb2d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb2d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb2d4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb2d4-110">Permission type</span></span>      | <span data-ttu-id="bb2d4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb2d4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb2d4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb2d4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bb2d4-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb2d4-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb2d4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb2d4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb2d4-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb2d4-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="bb2d4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb2d4-116">Application</span></span> | <span data-ttu-id="bb2d4-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb2d4-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb2d4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb2d4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="bb2d4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb2d4-119">Request headers</span></span>
| <span data-ttu-id="bb2d4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bb2d4-120">Name</span></span>       | <span data-ttu-id="bb2d4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb2d4-121">Type</span></span> | <span data-ttu-id="bb2d4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb2d4-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bb2d4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb2d4-123">Authorization</span></span>  | <span data-ttu-id="bb2d4-124">string</span><span class="sxs-lookup"><span data-stu-id="bb2d4-124">string</span></span>  | <span data-ttu-id="bb2d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb2d4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb2d4-127">Content-Type</span></span> | <span data-ttu-id="bb2d4-128">string</span><span class="sxs-lookup"><span data-stu-id="bb2d4-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="bb2d4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb2d4-129">Request body</span></span>
<span data-ttu-id="bb2d4-130">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="bb2d4-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bb2d4-131">Parameter</span></span>    | <span data-ttu-id="bb2d4-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb2d4-132">Type</span></span>   |<span data-ttu-id="bb2d4-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb2d4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb2d4-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="bb2d4-134">siteCollectionId</span></span>|<span data-ttu-id="bb2d4-135">String</span><span class="sxs-lookup"><span data-stu-id="bb2d4-135">String</span></span>|<span data-ttu-id="bb2d4-136">A ID do site do SharePoint para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="bb2d4-137">Use somente ao copiar para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="bb2d4-138">siteId</span><span class="sxs-lookup"><span data-stu-id="bb2d4-138">siteId</span></span>|<span data-ttu-id="bb2d4-139">String</span><span class="sxs-lookup"><span data-stu-id="bb2d4-139">String</span></span>|<span data-ttu-id="bb2d4-140">A ID da Web do SharePoint a ser copiada.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="bb2d4-141">Use somente ao copiar para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="bb2d4-142">groupId</span><span class="sxs-lookup"><span data-stu-id="bb2d4-142">groupId</span></span>|<span data-ttu-id="bb2d4-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb2d4-143">String</span></span>|<span data-ttu-id="bb2d4-144">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-144">The id of the group to copy to.</span></span> <span data-ttu-id="bb2d4-145">Use somente ao copiar para um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="bb2d4-146">id</span><span class="sxs-lookup"><span data-stu-id="bb2d4-146">id</span></span>|<span data-ttu-id="bb2d4-147">String</span><span class="sxs-lookup"><span data-stu-id="bb2d4-147">String</span></span>|<span data-ttu-id="bb2d4-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-148">Required.</span></span> <span data-ttu-id="bb2d4-149">A ID do grupo de seção de destino.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-149">The id of the destination section group.</span></span> |
|<span data-ttu-id="bb2d4-150">renomeas</span><span class="sxs-lookup"><span data-stu-id="bb2d4-150">renameAs</span></span>|<span data-ttu-id="bb2d4-151">String</span><span class="sxs-lookup"><span data-stu-id="bb2d4-151">String</span></span>|<span data-ttu-id="bb2d4-152">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-152">The name of the copy.</span></span> <span data-ttu-id="bb2d4-153">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-153">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="bb2d4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb2d4-154">Response</span></span>

<span data-ttu-id="bb2d4-155">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um `Operation-Location` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-155">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="bb2d4-156">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="bb2d4-156">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="bb2d4-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb2d4-157">Example</span></span>
<span data-ttu-id="bb2d4-158">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bb2d4-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb2d4-159">Request</span></span>
<span data-ttu-id="bb2d4-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb2d4-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb2d4-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="bb2d4-162">C#</span><span class="sxs-lookup"><span data-stu-id="bb2d4-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb2d4-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb2d4-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb2d4-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb2d4-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb2d4-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb2d4-165">Response</span></span>
<span data-ttu-id="bb2d4-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb2d4-166">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
