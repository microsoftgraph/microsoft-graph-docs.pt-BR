---
title: 'seção: copyToSectionGroup'
description: Copia uma seção para um grupo de seção específico.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 7a916903a995badede8dba872e11614664151373
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788042"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="ff47b-103">seção: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="ff47b-103">section: copyToSectionGroup</span></span>

<span data-ttu-id="ff47b-104">Namespace: microsoft.graph Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="ff47b-104">Namespace: microsoft.graph Copies a section to a specific section group.</span></span>

<span data-ttu-id="ff47b-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro chame a ação Copiar e, em seguida, sonda o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="ff47b-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff47b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff47b-106">Permissions</span></span>
<span data-ttu-id="ff47b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff47b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff47b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff47b-109">Permission type</span></span>      | <span data-ttu-id="ff47b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff47b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff47b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff47b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ff47b-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff47b-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff47b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff47b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff47b-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff47b-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ff47b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff47b-115">Application</span></span> | <span data-ttu-id="ff47b-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff47b-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff47b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff47b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="ff47b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff47b-118">Request headers</span></span>
| <span data-ttu-id="ff47b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ff47b-119">Name</span></span>       | <span data-ttu-id="ff47b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff47b-120">Type</span></span> | <span data-ttu-id="ff47b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff47b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff47b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff47b-122">Authorization</span></span>  | <span data-ttu-id="ff47b-123">string</span><span class="sxs-lookup"><span data-stu-id="ff47b-123">string</span></span>  | <span data-ttu-id="ff47b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff47b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff47b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff47b-126">Content-Type</span></span> | <span data-ttu-id="ff47b-127">string</span><span class="sxs-lookup"><span data-stu-id="ff47b-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ff47b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff47b-128">Request body</span></span>
<span data-ttu-id="ff47b-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="ff47b-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="ff47b-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ff47b-130">Parameter</span></span>    | <span data-ttu-id="ff47b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff47b-131">Type</span></span>   |<span data-ttu-id="ff47b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff47b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff47b-133">groupId</span><span class="sxs-lookup"><span data-stu-id="ff47b-133">groupId</span></span>|<span data-ttu-id="ff47b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff47b-134">String</span></span>|<span data-ttu-id="ff47b-135">A id do grupo para o que copiar.</span><span class="sxs-lookup"><span data-stu-id="ff47b-135">The id of the group to copy to.</span></span> <span data-ttu-id="ff47b-136">Use somente ao copiar para um Microsoft 365 grupo.</span><span class="sxs-lookup"><span data-stu-id="ff47b-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="ff47b-137">id</span><span class="sxs-lookup"><span data-stu-id="ff47b-137">id</span></span>|<span data-ttu-id="ff47b-138">String</span><span class="sxs-lookup"><span data-stu-id="ff47b-138">String</span></span>|<span data-ttu-id="ff47b-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff47b-139">Required.</span></span> <span data-ttu-id="ff47b-140">A id do grupo de seção de destino.</span><span class="sxs-lookup"><span data-stu-id="ff47b-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="ff47b-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="ff47b-141">renameAs</span></span>|<span data-ttu-id="ff47b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff47b-142">String</span></span>|<span data-ttu-id="ff47b-143">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="ff47b-143">The name of the copy.</span></span> <span data-ttu-id="ff47b-144">Padrão para o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="ff47b-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="ff47b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff47b-145">Response</span></span>

<span data-ttu-id="ff47b-146">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e um `Operation-Location` header.</span><span class="sxs-lookup"><span data-stu-id="ff47b-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="ff47b-147">Sondar Operation-Location ponto de extremidade para [obter o status da operação de cópia.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="ff47b-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="ff47b-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff47b-148">Example</span></span>
<span data-ttu-id="ff47b-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ff47b-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ff47b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff47b-150">Request</span></span>
<span data-ttu-id="ff47b-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff47b-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff47b-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff47b-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ff47b-153">C#</span><span class="sxs-lookup"><span data-stu-id="ff47b-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff47b-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff47b-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff47b-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff47b-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff47b-156">Java</span><span class="sxs-lookup"><span data-stu-id="ff47b-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytosectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff47b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff47b-157">Response</span></span>
<span data-ttu-id="ff47b-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff47b-158">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

