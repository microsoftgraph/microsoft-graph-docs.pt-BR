---
title: 'seção: copyToSectionGroup'
description: Copia uma seção para um grupo de seção específico.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 68a15f81fc61868d2f1b835c3a593a39be2546e3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897495"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="ad29e-103">seção: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="ad29e-103">section: copyToSectionGroup</span></span>

<span data-ttu-id="ad29e-104">Namespace: o Microsoft. Graph copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="ad29e-104">Namespace: microsoft.graph Copies a section to a specific section group.</span></span>

<span data-ttu-id="ad29e-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="ad29e-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad29e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad29e-106">Permissions</span></span>
<span data-ttu-id="ad29e-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ad29e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ad29e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad29e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad29e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad29e-109">Permission type</span></span>      | <span data-ttu-id="ad29e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad29e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad29e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad29e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad29e-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad29e-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad29e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad29e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad29e-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad29e-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ad29e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad29e-115">Application</span></span> | <span data-ttu-id="ad29e-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad29e-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad29e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad29e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="ad29e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad29e-118">Request headers</span></span>
| <span data-ttu-id="ad29e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ad29e-119">Name</span></span>       | <span data-ttu-id="ad29e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad29e-120">Type</span></span> | <span data-ttu-id="ad29e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad29e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ad29e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad29e-122">Authorization</span></span>  | <span data-ttu-id="ad29e-123">string</span><span class="sxs-lookup"><span data-stu-id="ad29e-123">string</span></span>  | <span data-ttu-id="ad29e-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="ad29e-124">Bearer {token}.</span></span> <span data-ttu-id="ad29e-125">Required.</span><span class="sxs-lookup"><span data-stu-id="ad29e-125">Required.</span></span> |
| <span data-ttu-id="ad29e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad29e-126">Content-Type</span></span> | <span data-ttu-id="ad29e-127">string</span><span class="sxs-lookup"><span data-stu-id="ad29e-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ad29e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad29e-128">Request body</span></span>
<span data-ttu-id="ad29e-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="ad29e-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="ad29e-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ad29e-130">Parameter</span></span>    | <span data-ttu-id="ad29e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad29e-131">Type</span></span>   |<span data-ttu-id="ad29e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad29e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad29e-133">groupId</span><span class="sxs-lookup"><span data-stu-id="ad29e-133">groupId</span></span>|<span data-ttu-id="ad29e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad29e-134">String</span></span>|<span data-ttu-id="ad29e-135">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="ad29e-135">The id of the group to copy to.</span></span> <span data-ttu-id="ad29e-136">Use somente ao copiar para um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ad29e-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="ad29e-137">id</span><span class="sxs-lookup"><span data-stu-id="ad29e-137">id</span></span>|<span data-ttu-id="ad29e-138">String</span><span class="sxs-lookup"><span data-stu-id="ad29e-138">String</span></span>|<span data-ttu-id="ad29e-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad29e-139">Required.</span></span> <span data-ttu-id="ad29e-140">A ID do grupo de seção de destino.</span><span class="sxs-lookup"><span data-stu-id="ad29e-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="ad29e-141">renomeas</span><span class="sxs-lookup"><span data-stu-id="ad29e-141">renameAs</span></span>|<span data-ttu-id="ad29e-142">String</span><span class="sxs-lookup"><span data-stu-id="ad29e-142">String</span></span>|<span data-ttu-id="ad29e-143">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="ad29e-143">The name of the copy.</span></span> <span data-ttu-id="ad29e-144">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="ad29e-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="ad29e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad29e-145">Response</span></span>

<span data-ttu-id="ad29e-146">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um `Operation-Location` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="ad29e-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="ad29e-147">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="ad29e-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="ad29e-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad29e-148">Example</span></span>
<span data-ttu-id="ad29e-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ad29e-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ad29e-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad29e-150">Request</span></span>
<span data-ttu-id="ad29e-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad29e-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad29e-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad29e-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ad29e-153">C#</span><span class="sxs-lookup"><span data-stu-id="ad29e-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad29e-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad29e-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad29e-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad29e-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad29e-156">Java</span><span class="sxs-lookup"><span data-stu-id="ad29e-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytosectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ad29e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad29e-157">Response</span></span>
<span data-ttu-id="ad29e-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad29e-158">Here is an example of the response.</span></span>
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
