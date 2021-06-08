---
title: 'bloco de anotações: copyNotebook'
description: Copia um bloco de anotações para a pasta Blocos de Anotações na biblioteca de documentos de destino. A pasta será criada se ela não existir.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: f46e65f200e87d0f39ef5e9307ee199de5595fb1
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787454"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="cd823-104">bloco de anotações: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="cd823-104">notebook: copyNotebook</span></span>

<span data-ttu-id="cd823-105">Namespace: microsoft.graph Copia um bloco de anotações para a pasta Blocos de Anotações na biblioteca de documentos de destino.</span><span class="sxs-lookup"><span data-stu-id="cd823-105">Namespace: microsoft.graph Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="cd823-106">A pasta será criada se ela não existir.</span><span class="sxs-lookup"><span data-stu-id="cd823-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="cd823-107">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro chame a ação Copiar e, em seguida, sonda o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="cd823-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd823-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd823-108">Permissions</span></span>
<span data-ttu-id="cd823-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd823-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd823-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd823-111">Permission type</span></span>      | <span data-ttu-id="cd823-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd823-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd823-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd823-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cd823-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd823-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd823-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd823-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd823-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd823-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="cd823-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd823-117">Application</span></span> | <span data-ttu-id="cd823-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd823-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd823-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd823-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="cd823-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd823-120">Request headers</span></span>
| <span data-ttu-id="cd823-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cd823-121">Name</span></span>       | <span data-ttu-id="cd823-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd823-122">Type</span></span> | <span data-ttu-id="cd823-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd823-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cd823-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd823-124">Authorization</span></span>  | <span data-ttu-id="cd823-125">string</span><span class="sxs-lookup"><span data-stu-id="cd823-125">string</span></span>  | <span data-ttu-id="cd823-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd823-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd823-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd823-128">Content-Type</span></span> | <span data-ttu-id="cd823-129">string</span><span class="sxs-lookup"><span data-stu-id="cd823-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="cd823-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd823-130">Request body</span></span>
<span data-ttu-id="cd823-131">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="cd823-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="cd823-132">Não há problema em enviar um corpo vazio se nenhum for necessário.</span><span class="sxs-lookup"><span data-stu-id="cd823-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="cd823-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cd823-133">Parameter</span></span>    | <span data-ttu-id="cd823-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd823-134">Type</span></span>   |<span data-ttu-id="cd823-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd823-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd823-136">groupId</span><span class="sxs-lookup"><span data-stu-id="cd823-136">groupId</span></span>|<span data-ttu-id="cd823-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd823-137">String</span></span>|<span data-ttu-id="cd823-138">A id do grupo para o que copiar.</span><span class="sxs-lookup"><span data-stu-id="cd823-138">The id of the group to copy to.</span></span> <span data-ttu-id="cd823-139">Use somente ao copiar para um Microsoft 365 grupo.</span><span class="sxs-lookup"><span data-stu-id="cd823-139">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="cd823-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="cd823-140">renameAs</span></span>|<span data-ttu-id="cd823-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd823-141">String</span></span>|<span data-ttu-id="cd823-142">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="cd823-142">The name of the copy.</span></span> <span data-ttu-id="cd823-143">Padrão para o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="cd823-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="cd823-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd823-144">Response</span></span>

<span data-ttu-id="cd823-145">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e um `Operation-Location` header.</span><span class="sxs-lookup"><span data-stu-id="cd823-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="cd823-146">Sondar Operation-Location ponto de extremidade para [obter o status da operação de cópia.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="cd823-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="cd823-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd823-147">Example</span></span>
<span data-ttu-id="cd823-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="cd823-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cd823-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd823-149">Request</span></span>
<span data-ttu-id="cd823-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd823-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd823-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd823-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="cd823-152">C#</span><span class="sxs-lookup"><span data-stu-id="cd823-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd823-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd823-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd823-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd823-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd823-155">Java</span><span class="sxs-lookup"><span data-stu-id="cd823-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cd823-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd823-156">Response</span></span>
<span data-ttu-id="cd823-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd823-157">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

