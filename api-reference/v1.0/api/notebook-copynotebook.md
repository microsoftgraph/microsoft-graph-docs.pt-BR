---
title: 'bloco de anotações: copyNotebook'
description: Copia um bloco de anotações para a pasta blocos de anotações na biblioteca de documentos de destino. A pasta é criada se não existir.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5f10c39cbb53da9329d11ee0724f716c28871813
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44892455"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="0fe54-104">bloco de anotações: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="0fe54-104">notebook: copyNotebook</span></span>

<span data-ttu-id="0fe54-105">Namespace: Microsoft. Graph copia um bloco de anotações para a pasta blocos de anotações na biblioteca de documentos de destino.</span><span class="sxs-lookup"><span data-stu-id="0fe54-105">Namespace: microsoft.graph Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="0fe54-106">A pasta é criada se não existir.</span><span class="sxs-lookup"><span data-stu-id="0fe54-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="0fe54-107">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="0fe54-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fe54-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fe54-108">Permissions</span></span>
<span data-ttu-id="0fe54-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fe54-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fe54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fe54-111">Permission type</span></span>      | <span data-ttu-id="0fe54-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fe54-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fe54-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fe54-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0fe54-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe54-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0fe54-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fe54-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fe54-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fe54-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0fe54-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fe54-117">Application</span></span> | <span data-ttu-id="0fe54-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe54-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fe54-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe54-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="0fe54-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe54-120">Request headers</span></span>
| <span data-ttu-id="0fe54-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0fe54-121">Name</span></span>       | <span data-ttu-id="0fe54-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fe54-122">Type</span></span> | <span data-ttu-id="0fe54-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fe54-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0fe54-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fe54-124">Authorization</span></span>  | <span data-ttu-id="0fe54-125">string</span><span class="sxs-lookup"><span data-stu-id="0fe54-125">string</span></span>  | <span data-ttu-id="0fe54-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fe54-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0fe54-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fe54-128">Content-Type</span></span> | <span data-ttu-id="0fe54-129">string</span><span class="sxs-lookup"><span data-stu-id="0fe54-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0fe54-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe54-130">Request body</span></span>
<span data-ttu-id="0fe54-131">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="0fe54-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="0fe54-132">É possível enviar um corpo vazio se nenhum for necessário.</span><span class="sxs-lookup"><span data-stu-id="0fe54-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="0fe54-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0fe54-133">Parameter</span></span>    | <span data-ttu-id="0fe54-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fe54-134">Type</span></span>   |<span data-ttu-id="0fe54-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fe54-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fe54-136">groupId</span><span class="sxs-lookup"><span data-stu-id="0fe54-136">groupId</span></span>|<span data-ttu-id="0fe54-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fe54-137">String</span></span>|<span data-ttu-id="0fe54-138">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="0fe54-138">The id of the group to copy to.</span></span> <span data-ttu-id="0fe54-139">Use somente ao copiar para um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0fe54-139">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="0fe54-140">renomeas</span><span class="sxs-lookup"><span data-stu-id="0fe54-140">renameAs</span></span>|<span data-ttu-id="0fe54-141">String</span><span class="sxs-lookup"><span data-stu-id="0fe54-141">String</span></span>|<span data-ttu-id="0fe54-142">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="0fe54-142">The name of the copy.</span></span> <span data-ttu-id="0fe54-143">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="0fe54-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="0fe54-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe54-144">Response</span></span>

<span data-ttu-id="0fe54-145">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um `Operation-Location` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="0fe54-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="0fe54-146">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="0fe54-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="0fe54-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fe54-147">Example</span></span>
<span data-ttu-id="0fe54-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0fe54-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0fe54-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe54-149">Request</span></span>
<span data-ttu-id="0fe54-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fe54-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fe54-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe54-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0fe54-152">C#</span><span class="sxs-lookup"><span data-stu-id="0fe54-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fe54-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fe54-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fe54-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fe54-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fe54-155">Java</span><span class="sxs-lookup"><span data-stu-id="0fe54-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0fe54-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe54-156">Response</span></span>
<span data-ttu-id="0fe54-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe54-157">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
