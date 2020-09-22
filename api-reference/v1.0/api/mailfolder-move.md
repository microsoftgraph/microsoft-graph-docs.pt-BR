---
title: 'mailFolder: move'
description: Mova uma mailFolder e seu conteúdo para outra mailFolder.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e689a77484aad7b2a6d1412c4a49e07f33ea0441
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033017"
---
# <a name="mailfolder-move"></a><span data-ttu-id="55156-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="55156-103">mailFolder: move</span></span>

<span data-ttu-id="55156-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55156-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55156-105">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="55156-105">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="55156-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55156-106">Permissions</span></span>

<span data-ttu-id="55156-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55156-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55156-109">Permission type</span></span> | <span data-ttu-id="55156-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55156-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="55156-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55156-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55156-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55156-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="55156-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55156-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55156-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55156-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="55156-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55156-115">Application</span></span> | <span data-ttu-id="55156-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55156-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="55156-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55156-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="55156-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55156-118">Request headers</span></span>

| <span data-ttu-id="55156-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55156-119">Header</span></span> | <span data-ttu-id="55156-120">Valor</span><span class="sxs-lookup"><span data-stu-id="55156-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="55156-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="55156-121">Authorization</span></span> | <span data-ttu-id="55156-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="55156-122">`Bearer {token}`.</span></span> <span data-ttu-id="55156-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55156-123">Required.</span></span> |
| <span data-ttu-id="55156-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55156-124">Content-Type</span></span> | <span data-ttu-id="55156-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="55156-125">`application/json`.</span></span> <span data-ttu-id="55156-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55156-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55156-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55156-127">Request body</span></span>

<span data-ttu-id="55156-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55156-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55156-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="55156-129">Parameter</span></span> | <span data-ttu-id="55156-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="55156-130">Type</span></span> | <span data-ttu-id="55156-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="55156-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="55156-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="55156-132">destinationId</span></span>|<span data-ttu-id="55156-133">String</span><span class="sxs-lookup"><span data-stu-id="55156-133">String</span></span>|<span data-ttu-id="55156-134">A ID da pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="55156-134">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="55156-135">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="55156-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="55156-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="55156-136">Response</span></span>

<span data-ttu-id="55156-137">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55156-137">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55156-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55156-138">Example</span></span>

<span data-ttu-id="55156-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="55156-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="55156-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55156-140">Request</span></span>

<span data-ttu-id="55156-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55156-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55156-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="55156-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="55156-143">C#</span><span class="sxs-lookup"><span data-stu-id="55156-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55156-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55156-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55156-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55156-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55156-146">Java</span><span class="sxs-lookup"><span data-stu-id="55156-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-move-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55156-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="55156-147">Response</span></span>

<span data-ttu-id="55156-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55156-148">Here is an example of the response.</span></span>

> <span data-ttu-id="55156-149">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55156-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55156-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55156-150">All the properties will be returned from an actual call.</span></span>
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

