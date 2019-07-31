---
title: 'bloco de anotações: copyNotebook'
description: Copia um bloco de anotações para a pasta blocos de anotações na biblioteca de documentos de destino. A pasta é criada se não existir.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 38c8bc918b49ee6e4da5ed7ff921d1f661a0c4a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983737"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="dccdc-104">bloco de anotações: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="dccdc-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dccdc-105">Copia um bloco de anotações para a pasta blocos de anotações na biblioteca de documentos de destino.</span><span class="sxs-lookup"><span data-stu-id="dccdc-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="dccdc-106">A pasta é criada se não existir.</span><span class="sxs-lookup"><span data-stu-id="dccdc-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="dccdc-107">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="dccdc-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="dccdc-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dccdc-108">Permissions</span></span>
<span data-ttu-id="dccdc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dccdc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dccdc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dccdc-111">Permission type</span></span>      | <span data-ttu-id="dccdc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dccdc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dccdc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dccdc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dccdc-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dccdc-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="dccdc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dccdc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dccdc-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dccdc-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="dccdc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dccdc-117">Application</span></span> | <span data-ttu-id="dccdc-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dccdc-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dccdc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dccdc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="dccdc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dccdc-120">Request headers</span></span>
| <span data-ttu-id="dccdc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dccdc-121">Name</span></span>       | <span data-ttu-id="dccdc-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="dccdc-122">Type</span></span> | <span data-ttu-id="dccdc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="dccdc-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dccdc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dccdc-124">Authorization</span></span>  | <span data-ttu-id="dccdc-125">string</span><span class="sxs-lookup"><span data-stu-id="dccdc-125">string</span></span>  | <span data-ttu-id="dccdc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dccdc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dccdc-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dccdc-128">Content-Type</span></span> | <span data-ttu-id="dccdc-129">string</span><span class="sxs-lookup"><span data-stu-id="dccdc-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="dccdc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dccdc-130">Request body</span></span>
<span data-ttu-id="dccdc-131">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="dccdc-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="dccdc-132">É possível enviar um corpo vazio se nenhum for necessário.</span><span class="sxs-lookup"><span data-stu-id="dccdc-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="dccdc-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dccdc-133">Parameter</span></span>    | <span data-ttu-id="dccdc-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="dccdc-134">Type</span></span>   |<span data-ttu-id="dccdc-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="dccdc-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dccdc-136">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="dccdc-136">siteCollectionId</span></span>|<span data-ttu-id="dccdc-137">String</span><span class="sxs-lookup"><span data-stu-id="dccdc-137">String</span></span>|<span data-ttu-id="dccdc-138">A ID do site do SharePoint para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="dccdc-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="dccdc-139">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="dccdc-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="dccdc-140">siteId</span><span class="sxs-lookup"><span data-stu-id="dccdc-140">siteId</span></span>|<span data-ttu-id="dccdc-141">String</span><span class="sxs-lookup"><span data-stu-id="dccdc-141">String</span></span>|<span data-ttu-id="dccdc-142">A ID da Web do SharePoint a ser copiada.</span><span class="sxs-lookup"><span data-stu-id="dccdc-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="dccdc-143">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="dccdc-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="dccdc-144">groupId</span><span class="sxs-lookup"><span data-stu-id="dccdc-144">groupId</span></span>|<span data-ttu-id="dccdc-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dccdc-145">String</span></span>|<span data-ttu-id="dccdc-146">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="dccdc-146">The id of the group to copy to.</span></span> <span data-ttu-id="dccdc-147">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="dccdc-147">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="dccdc-148">renomeas</span><span class="sxs-lookup"><span data-stu-id="dccdc-148">renameAs</span></span>|<span data-ttu-id="dccdc-149">String</span><span class="sxs-lookup"><span data-stu-id="dccdc-149">String</span></span>|<span data-ttu-id="dccdc-150">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="dccdc-150">The name of the copy.</span></span> <span data-ttu-id="dccdc-151">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="dccdc-151">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="dccdc-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="dccdc-152">Response</span></span>

<span data-ttu-id="dccdc-153">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="dccdc-153">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="dccdc-154">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="dccdc-154">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="dccdc-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dccdc-155">Example</span></span>
<span data-ttu-id="dccdc-156">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dccdc-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dccdc-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dccdc-157">Request</span></span>
<span data-ttu-id="dccdc-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dccdc-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dccdc-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="dccdc-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="dccdc-160">C#</span><span class="sxs-lookup"><span data-stu-id="dccdc-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dccdc-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="dccdc-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dccdc-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dccdc-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dccdc-163">Java</span><span class="sxs-lookup"><span data-stu-id="dccdc-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dccdc-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="dccdc-164">Response</span></span>
<span data-ttu-id="dccdc-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dccdc-165">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
