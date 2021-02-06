---
title: 'mailFolder: copy'
description: Copie uma mailFolder e seu conteúdo para outra mailFolder.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 879ef908599321d51e1537115fc66f2e3a38c663
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136784"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="9f84b-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="9f84b-103">mailFolder: copy</span></span>

<span data-ttu-id="9f84b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f84b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f84b-105">Copie uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="9f84b-105">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f84b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f84b-106">Permissions</span></span>

<span data-ttu-id="9f84b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f84b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f84b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f84b-109">Permission type</span></span> | <span data-ttu-id="9f84b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f84b-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="9f84b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f84b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f84b-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f84b-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f84b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f84b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f84b-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f84b-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f84b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f84b-115">Application</span></span> | <span data-ttu-id="9f84b-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f84b-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f84b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f84b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="9f84b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f84b-118">Request headers</span></span>

| <span data-ttu-id="9f84b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f84b-119">Header</span></span> | <span data-ttu-id="9f84b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9f84b-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="9f84b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f84b-121">Authorization</span></span> | <span data-ttu-id="9f84b-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="9f84b-122">`Bearer {token}`.</span></span> <span data-ttu-id="9f84b-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f84b-123">Required.</span></span> |
| <span data-ttu-id="9f84b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f84b-124">Content-Type</span></span> | <span data-ttu-id="9f84b-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="9f84b-125">`application/json`.</span></span> <span data-ttu-id="9f84b-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f84b-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f84b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f84b-127">Request body</span></span>

<span data-ttu-id="9f84b-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f84b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9f84b-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9f84b-129">Parameter</span></span> | <span data-ttu-id="9f84b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f84b-130">Type</span></span> | <span data-ttu-id="9f84b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f84b-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="9f84b-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="9f84b-132">destinationId</span></span>|<span data-ttu-id="9f84b-133">String</span><span class="sxs-lookup"><span data-stu-id="9f84b-133">String</span></span>|<span data-ttu-id="9f84b-134">A ID da pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="9f84b-134">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="9f84b-135">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9f84b-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="9f84b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f84b-136">Response</span></span>

<span data-ttu-id="9f84b-137">Se bem-sucedido, este método retorna `200 OK` o código de resposta e um recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f84b-137">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f84b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f84b-138">Example</span></span>

<span data-ttu-id="9f84b-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9f84b-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9f84b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f84b-140">Request</span></span>

<span data-ttu-id="9f84b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f84b-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f84b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f84b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="9f84b-143">C#</span><span class="sxs-lookup"><span data-stu-id="9f84b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f84b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f84b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f84b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f84b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f84b-146">Java</span><span class="sxs-lookup"><span data-stu-id="9f84b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9f84b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f84b-147">Response</span></span>

<span data-ttu-id="9f84b-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f84b-148">Here is an example of the response.</span></span>

> <span data-ttu-id="9f84b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f84b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


