---
title: 'seção: copyToSectionGroup'
description: Copia uma seção para um grupo de seção específico.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9deb5c9003471026905457a910c6d966463df66b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021582"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="b231a-103">seção: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="b231a-103">section: copyToSectionGroup</span></span>
<span data-ttu-id="b231a-104">Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="b231a-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="b231a-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="b231a-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="b231a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b231a-106">Permissions</span></span>
<span data-ttu-id="b231a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b231a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b231a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b231a-109">Permission type</span></span>      | <span data-ttu-id="b231a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b231a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b231a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b231a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b231a-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b231a-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b231a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b231a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b231a-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b231a-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b231a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b231a-115">Application</span></span> | <span data-ttu-id="b231a-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b231a-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b231a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b231a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="b231a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b231a-118">Request headers</span></span>
| <span data-ttu-id="b231a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b231a-119">Name</span></span>       | <span data-ttu-id="b231a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b231a-120">Type</span></span> | <span data-ttu-id="b231a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b231a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b231a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b231a-122">Authorization</span></span>  | <span data-ttu-id="b231a-123">string</span><span class="sxs-lookup"><span data-stu-id="b231a-123">string</span></span>  | <span data-ttu-id="b231a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b231a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b231a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b231a-126">Content-Type</span></span> | <span data-ttu-id="b231a-127">string</span><span class="sxs-lookup"><span data-stu-id="b231a-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b231a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b231a-128">Request body</span></span>
<span data-ttu-id="b231a-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="b231a-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="b231a-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b231a-130">Parameter</span></span>    | <span data-ttu-id="b231a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b231a-131">Type</span></span>   |<span data-ttu-id="b231a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b231a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b231a-133">groupId</span><span class="sxs-lookup"><span data-stu-id="b231a-133">groupId</span></span>|<span data-ttu-id="b231a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b231a-134">String</span></span>|<span data-ttu-id="b231a-135">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="b231a-135">The id of the group to copy to.</span></span> <span data-ttu-id="b231a-136">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b231a-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="b231a-137">id</span><span class="sxs-lookup"><span data-stu-id="b231a-137">id</span></span>|<span data-ttu-id="b231a-138">String</span><span class="sxs-lookup"><span data-stu-id="b231a-138">String</span></span>|<span data-ttu-id="b231a-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b231a-139">Required.</span></span> <span data-ttu-id="b231a-140">A ID do grupo de seção de destino.</span><span class="sxs-lookup"><span data-stu-id="b231a-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="b231a-141">renomeas</span><span class="sxs-lookup"><span data-stu-id="b231a-141">renameAs</span></span>|<span data-ttu-id="b231a-142">String</span><span class="sxs-lookup"><span data-stu-id="b231a-142">String</span></span>|<span data-ttu-id="b231a-143">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="b231a-143">The name of the copy.</span></span> <span data-ttu-id="b231a-144">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="b231a-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="b231a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b231a-145">Response</span></span>

<span data-ttu-id="b231a-146">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="b231a-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="b231a-147">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="b231a-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b231a-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b231a-148">Example</span></span>
<span data-ttu-id="b231a-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b231a-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b231a-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b231a-150">Request</span></span>
<span data-ttu-id="b231a-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b231a-151">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b231a-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="b231a-152">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b231a-153">C#</span><span class="sxs-lookup"><span data-stu-id="b231a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b231a-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="b231a-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b231a-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b231a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b231a-156">Java</span><span class="sxs-lookup"><span data-stu-id="b231a-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytosectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b231a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b231a-157">Response</span></span>
<span data-ttu-id="b231a-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b231a-158">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
