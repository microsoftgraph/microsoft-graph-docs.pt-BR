---
title: Criar MailFolder
description: Use essa API para criar uma nova mailfolder filha.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7746fb03f6f47f81f0807cdc42e1b7af8a982cfe
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055929"
---
# <a name="create-mailfolder"></a><span data-ttu-id="c4b5a-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="c4b5a-103">Create MailFolder</span></span>

<span data-ttu-id="c4b5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4b5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4b5a-105">Use essa API para criar uma nova mailfolder filha.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-105">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4b5a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4b5a-106">Permissions</span></span>

<span data-ttu-id="c4b5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4b5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4b5a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4b5a-109">Permission type</span></span> | <span data-ttu-id="c4b5a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4b5a-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="c4b5a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4b5a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c4b5a-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4b5a-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c4b5a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4b5a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4b5a-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4b5a-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c4b5a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4b5a-115">Application</span></span> | <span data-ttu-id="c4b5a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4b5a-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4b5a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4b5a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="c4b5a-118">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="c4b5a-119">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c4b5a-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4b5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4b5a-120">Request headers</span></span>

| <span data-ttu-id="c4b5a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4b5a-121">Header</span></span> | <span data-ttu-id="c4b5a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4b5a-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="c4b5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4b5a-123">Authorization</span></span> | <span data-ttu-id="c4b5a-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-124">`Bearer {token}`.</span></span> <span data-ttu-id="c4b5a-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-125">Required.</span></span> |
| <span data-ttu-id="c4b5a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4b5a-126">Content-Type</span></span> | <span data-ttu-id="c4b5a-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-127">`application/json`.</span></span> <span data-ttu-id="c4b5a-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4b5a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4b5a-129">Request body</span></span>

<span data-ttu-id="c4b5a-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-130">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="c4b5a-131">**displayName** é a única propriedade writable para um [objeto mailFolder.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="c4b5a-131">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="c4b5a-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c4b5a-132">Parameter</span></span> | <span data-ttu-id="c4b5a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4b5a-133">Type</span></span> | <span data-ttu-id="c4b5a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4b5a-134">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="c4b5a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c4b5a-135">displayName</span></span>|<span data-ttu-id="c4b5a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4b5a-136">String</span></span>|<span data-ttu-id="c4b5a-137">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-137">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="c4b5a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4b5a-138">Response</span></span>

<span data-ttu-id="c4b5a-139">Se tiver êxito, este método retornará `201 Created` o código de resposta e um recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-139">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4b5a-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4b5a-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c4b5a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4b5a-141">Request</span></span>

<span data-ttu-id="c4b5a-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4b5a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4b5a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="c4b5a-144">C#</span><span class="sxs-lookup"><span data-stu-id="c4b5a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4b5a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4b5a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4b5a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4b5a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4b5a-147">Java</span><span class="sxs-lookup"><span data-stu-id="c4b5a-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4b5a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4b5a-148">Response</span></span>
<span data-ttu-id="c4b5a-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-149">Here is an example of the response.</span></span>

> <span data-ttu-id="c4b5a-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4b5a-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

