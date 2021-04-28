---
title: 'mailFolder: move'
description: Mova uma mailFolder e seu conteúdo para outra mailFolder.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 495735363e3c22bafceb31ed94fa794c324344fc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055936"
---
# <a name="mailfolder-move"></a><span data-ttu-id="4665c-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="4665c-103">mailFolder: move</span></span>

<span data-ttu-id="4665c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4665c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4665c-105">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="4665c-105">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="4665c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4665c-106">Permissions</span></span>

<span data-ttu-id="4665c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4665c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4665c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4665c-109">Permission type</span></span> | <span data-ttu-id="4665c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4665c-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="4665c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4665c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4665c-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4665c-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4665c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4665c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4665c-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4665c-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4665c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4665c-115">Application</span></span> | <span data-ttu-id="4665c-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4665c-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4665c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4665c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="4665c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4665c-118">Request headers</span></span>

| <span data-ttu-id="4665c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4665c-119">Header</span></span> | <span data-ttu-id="4665c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4665c-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="4665c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4665c-121">Authorization</span></span> | <span data-ttu-id="4665c-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="4665c-122">`Bearer {token}`.</span></span> <span data-ttu-id="4665c-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4665c-123">Required.</span></span> |
| <span data-ttu-id="4665c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4665c-124">Content-Type</span></span> | <span data-ttu-id="4665c-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="4665c-125">`application/json`.</span></span> <span data-ttu-id="4665c-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4665c-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4665c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4665c-127">Request body</span></span>

<span data-ttu-id="4665c-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4665c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4665c-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4665c-129">Parameter</span></span> | <span data-ttu-id="4665c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4665c-130">Type</span></span> | <span data-ttu-id="4665c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4665c-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="4665c-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="4665c-132">destinationId</span></span>|<span data-ttu-id="4665c-133">String</span><span class="sxs-lookup"><span data-stu-id="4665c-133">String</span></span>|<span data-ttu-id="4665c-134">A ID da pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="4665c-134">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="4665c-135">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="4665c-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="4665c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4665c-136">Response</span></span>

<span data-ttu-id="4665c-137">Se tiver êxito, este método retornará `200 OK` o código de resposta e um recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4665c-137">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4665c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4665c-138">Example</span></span>

<span data-ttu-id="4665c-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4665c-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4665c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4665c-140">Request</span></span>

<span data-ttu-id="4665c-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4665c-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4665c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4665c-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4665c-143">C#</span><span class="sxs-lookup"><span data-stu-id="4665c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4665c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4665c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4665c-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4665c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4665c-146">Java</span><span class="sxs-lookup"><span data-stu-id="4665c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-move-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4665c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4665c-147">Response</span></span>

<span data-ttu-id="4665c-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4665c-148">Here is an example of the response.</span></span>

> <span data-ttu-id="4665c-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4665c-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

