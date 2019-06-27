---
title: 'bloco de anotações: copyNotebook'
description: Copia um bloco de anotações para a pasta blocos de anotações na biblioteca de documentos de destino. A pasta é criada se não existir.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 01e5f0ec7edd898c53447eafe930cc72cc9561ad
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274582"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="d7247-104">bloco de anotações: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="d7247-104">notebook: copyNotebook</span></span>
<span data-ttu-id="d7247-105">Copia um bloco de anotações para a pasta blocos de anotações na biblioteca de documentos de destino.</span><span class="sxs-lookup"><span data-stu-id="d7247-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="d7247-106">A pasta é criada se não existir.</span><span class="sxs-lookup"><span data-stu-id="d7247-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="d7247-107">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="d7247-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7247-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7247-108">Permissions</span></span>
<span data-ttu-id="d7247-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7247-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7247-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7247-111">Permission type</span></span>      | <span data-ttu-id="d7247-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7247-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7247-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7247-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d7247-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7247-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7247-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7247-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7247-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7247-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d7247-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7247-117">Application</span></span> | <span data-ttu-id="d7247-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7247-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7247-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7247-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="d7247-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7247-120">Request headers</span></span>
| <span data-ttu-id="d7247-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d7247-121">Name</span></span>       | <span data-ttu-id="d7247-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7247-122">Type</span></span> | <span data-ttu-id="d7247-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7247-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d7247-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7247-124">Authorization</span></span>  | <span data-ttu-id="d7247-125">string</span><span class="sxs-lookup"><span data-stu-id="d7247-125">string</span></span>  | <span data-ttu-id="d7247-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7247-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7247-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7247-128">Content-Type</span></span> | <span data-ttu-id="d7247-129">string</span><span class="sxs-lookup"><span data-stu-id="d7247-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d7247-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7247-130">Request body</span></span>
<span data-ttu-id="d7247-131">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="d7247-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="d7247-132">É possível enviar um corpo vazio se nenhum for necessário.</span><span class="sxs-lookup"><span data-stu-id="d7247-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="d7247-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d7247-133">Parameter</span></span>    | <span data-ttu-id="d7247-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7247-134">Type</span></span>   |<span data-ttu-id="d7247-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7247-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7247-136">groupId</span><span class="sxs-lookup"><span data-stu-id="d7247-136">groupId</span></span>|<span data-ttu-id="d7247-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7247-137">String</span></span>|<span data-ttu-id="d7247-138">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="d7247-138">The id of the group to copy to.</span></span> <span data-ttu-id="d7247-139">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d7247-139">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="d7247-140">renomeas</span><span class="sxs-lookup"><span data-stu-id="d7247-140">renameAs</span></span>|<span data-ttu-id="d7247-141">String</span><span class="sxs-lookup"><span data-stu-id="d7247-141">String</span></span>|<span data-ttu-id="d7247-142">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="d7247-142">The name of the copy.</span></span> <span data-ttu-id="d7247-143">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="d7247-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="d7247-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7247-144">Response</span></span>

<span data-ttu-id="d7247-145">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="d7247-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="d7247-146">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="d7247-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="d7247-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7247-147">Example</span></span>
<span data-ttu-id="d7247-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d7247-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7247-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7247-149">Request</span></span>
<span data-ttu-id="d7247-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7247-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d7247-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7247-151">Response</span></span>
<span data-ttu-id="d7247-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7247-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d7247-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d7247-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d7247-154">C#</span><span class="sxs-lookup"><span data-stu-id="d7247-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7247-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="d7247-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d7247-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d7247-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
