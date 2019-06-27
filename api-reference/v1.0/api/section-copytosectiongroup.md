---
title: 'seção: copyToSectionGroup'
description: Copia uma seção para um grupo de seção específico.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 34455921995768ba9d2faffac3319cb1d58b5d64
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279300"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="efea3-103">seção: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="efea3-103">section: copyToSectionGroup</span></span>
<span data-ttu-id="efea3-104">Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="efea3-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="efea3-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="efea3-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="efea3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="efea3-106">Permissions</span></span>
<span data-ttu-id="efea3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efea3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efea3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efea3-109">Permission type</span></span>      | <span data-ttu-id="efea3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efea3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efea3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efea3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="efea3-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efea3-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="efea3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efea3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efea3-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efea3-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="efea3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efea3-115">Application</span></span> | <span data-ttu-id="efea3-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efea3-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efea3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efea3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="efea3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efea3-118">Request headers</span></span>
| <span data-ttu-id="efea3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="efea3-119">Name</span></span>       | <span data-ttu-id="efea3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="efea3-120">Type</span></span> | <span data-ttu-id="efea3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="efea3-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="efea3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="efea3-122">Authorization</span></span>  | <span data-ttu-id="efea3-123">string</span><span class="sxs-lookup"><span data-stu-id="efea3-123">string</span></span>  | <span data-ttu-id="efea3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efea3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="efea3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="efea3-126">Content-Type</span></span> | <span data-ttu-id="efea3-127">string</span><span class="sxs-lookup"><span data-stu-id="efea3-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="efea3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efea3-128">Request body</span></span>
<span data-ttu-id="efea3-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="efea3-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="efea3-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="efea3-130">Parameter</span></span>    | <span data-ttu-id="efea3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efea3-131">Type</span></span>   |<span data-ttu-id="efea3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efea3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efea3-133">groupId</span><span class="sxs-lookup"><span data-stu-id="efea3-133">groupId</span></span>|<span data-ttu-id="efea3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efea3-134">String</span></span>|<span data-ttu-id="efea3-135">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="efea3-135">The id of the group to copy to.</span></span> <span data-ttu-id="efea3-136">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="efea3-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="efea3-137">id</span><span class="sxs-lookup"><span data-stu-id="efea3-137">id</span></span>|<span data-ttu-id="efea3-138">String</span><span class="sxs-lookup"><span data-stu-id="efea3-138">String</span></span>|<span data-ttu-id="efea3-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efea3-139">Required.</span></span> <span data-ttu-id="efea3-140">A ID do grupo de seção de destino.</span><span class="sxs-lookup"><span data-stu-id="efea3-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="efea3-141">renomeas</span><span class="sxs-lookup"><span data-stu-id="efea3-141">renameAs</span></span>|<span data-ttu-id="efea3-142">String</span><span class="sxs-lookup"><span data-stu-id="efea3-142">String</span></span>|<span data-ttu-id="efea3-143">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="efea3-143">The name of the copy.</span></span> <span data-ttu-id="efea3-144">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="efea3-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="efea3-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="efea3-145">Response</span></span>

<span data-ttu-id="efea3-146">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="efea3-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="efea3-147">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="efea3-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="efea3-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efea3-148">Example</span></span>
<span data-ttu-id="efea3-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="efea3-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="efea3-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efea3-150">Request</span></span>
<span data-ttu-id="efea3-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efea3-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="efea3-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="efea3-152">Response</span></span>
<span data-ttu-id="efea3-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efea3-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="efea3-154">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="efea3-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="efea3-155">C#</span><span class="sxs-lookup"><span data-stu-id="efea3-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="efea3-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="efea3-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="efea3-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="efea3-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
