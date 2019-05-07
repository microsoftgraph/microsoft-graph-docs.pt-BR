---
title: 'seção: copyToNotebook'
description: Copia uma seção para um bloco de anotações específico.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ed7285f601d0509404ecab73a2029e9f55212971
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603568"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="649d6-103">seção: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="649d6-103">section: copyToNotebook</span></span>
<span data-ttu-id="649d6-104">Copia uma seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="649d6-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="649d6-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="649d6-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="649d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="649d6-106">Permissions</span></span>
<span data-ttu-id="649d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="649d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="649d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="649d6-109">Permission type</span></span>      | <span data-ttu-id="649d6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="649d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="649d6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="649d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="649d6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="649d6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="649d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="649d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="649d6-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="649d6-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="649d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="649d6-115">Application</span></span> | <span data-ttu-id="649d6-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="649d6-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="649d6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="649d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="649d6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="649d6-118">Request headers</span></span>
| <span data-ttu-id="649d6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="649d6-119">Name</span></span>       | <span data-ttu-id="649d6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="649d6-120">Type</span></span> | <span data-ttu-id="649d6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="649d6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="649d6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="649d6-122">Authorization</span></span>  | <span data-ttu-id="649d6-123">string</span><span class="sxs-lookup"><span data-stu-id="649d6-123">string</span></span>  | <span data-ttu-id="649d6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="649d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="649d6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="649d6-126">Content-Type</span></span> | <span data-ttu-id="649d6-127">string</span><span class="sxs-lookup"><span data-stu-id="649d6-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="649d6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="649d6-128">Request body</span></span>
<span data-ttu-id="649d6-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="649d6-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="649d6-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="649d6-130">Parameter</span></span>    | <span data-ttu-id="649d6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="649d6-131">Type</span></span>   |<span data-ttu-id="649d6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="649d6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="649d6-133">groupId</span><span class="sxs-lookup"><span data-stu-id="649d6-133">groupId</span></span>|<span data-ttu-id="649d6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="649d6-134">String</span></span>|<span data-ttu-id="649d6-135">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="649d6-135">The id of the group to copy to.</span></span> <span data-ttu-id="649d6-136">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="649d6-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="649d6-137">id</span><span class="sxs-lookup"><span data-stu-id="649d6-137">id</span></span>|<span data-ttu-id="649d6-138">String</span><span class="sxs-lookup"><span data-stu-id="649d6-138">String</span></span>|<span data-ttu-id="649d6-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="649d6-139">Required.</span></span> <span data-ttu-id="649d6-140">A ID do bloco de anotações de destino.</span><span class="sxs-lookup"><span data-stu-id="649d6-140">The id of the destination notebook.</span></span> |
|<span data-ttu-id="649d6-141">renomeas</span><span class="sxs-lookup"><span data-stu-id="649d6-141">renameAs</span></span>|<span data-ttu-id="649d6-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="649d6-142">String</span></span>|<span data-ttu-id="649d6-143">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="649d6-143">The name of the copy.</span></span> <span data-ttu-id="649d6-144">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="649d6-144">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="649d6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="649d6-145">Response</span></span>

<span data-ttu-id="649d6-146">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="649d6-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="649d6-147">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="649d6-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="649d6-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="649d6-148">Example</span></span>
<span data-ttu-id="649d6-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="649d6-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="649d6-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="649d6-150">Request</span></span>
<span data-ttu-id="649d6-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="649d6-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="649d6-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="649d6-152">Response</span></span>
<span data-ttu-id="649d6-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="649d6-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="649d6-154">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="649d6-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="649d6-155">Basic</span><span class="sxs-lookup"><span data-stu-id="649d6-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/section_copytonotebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="649d6-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="649d6-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/section_copytonotebook-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/section-copytonotebook.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/section-copytonotebook.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
