---
title: Criar MailFolder
description: Use essa API para criar um novo mailFolder filho.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8d79b9817332c7aea773ad9062efd3a4718dd197
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049251"
---
# <a name="create-mailfolder"></a><span data-ttu-id="6af68-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="6af68-103">Create mailFolder</span></span>

<span data-ttu-id="6af68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6af68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6af68-105">Use essa API para criar um novo [mailFolder filho.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="6af68-105">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6af68-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6af68-106">Permissions</span></span>

<span data-ttu-id="6af68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6af68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6af68-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6af68-109">Permission type</span></span> | <span data-ttu-id="6af68-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6af68-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="6af68-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6af68-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6af68-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6af68-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6af68-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6af68-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6af68-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6af68-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6af68-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6af68-115">Application</span></span> | <span data-ttu-id="6af68-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6af68-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6af68-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6af68-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="6af68-118">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="6af68-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="6af68-119">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6af68-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6af68-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6af68-120">Request headers</span></span>

| <span data-ttu-id="6af68-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6af68-121">Header</span></span> | <span data-ttu-id="6af68-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6af68-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="6af68-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6af68-123">Authorization</span></span> | <span data-ttu-id="6af68-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="6af68-124">`Bearer {token}`.</span></span> <span data-ttu-id="6af68-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6af68-125">Required.</span></span> |
| <span data-ttu-id="6af68-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6af68-126">Content-Type</span></span> | <span data-ttu-id="6af68-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="6af68-127">`application/json`.</span></span> <span data-ttu-id="6af68-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6af68-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6af68-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6af68-129">Request body</span></span>

<span data-ttu-id="6af68-p105">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6af68-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="6af68-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6af68-132">Parameter</span></span> | <span data-ttu-id="6af68-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="6af68-133">Type</span></span> | <span data-ttu-id="6af68-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6af68-134">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="6af68-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6af68-135">displayName</span></span>|<span data-ttu-id="6af68-136">String</span><span class="sxs-lookup"><span data-stu-id="6af68-136">String</span></span>|<span data-ttu-id="6af68-137">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="6af68-137">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="6af68-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af68-138">Response</span></span>

<span data-ttu-id="6af68-139">Se tiver êxito, este método retornará `201 Created` o código de resposta e um objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6af68-139">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6af68-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6af68-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6af68-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6af68-141">Request</span></span>

<span data-ttu-id="6af68-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6af68-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6af68-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6af68-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="6af68-144">C#</span><span class="sxs-lookup"><span data-stu-id="6af68-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6af68-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6af68-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6af68-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6af68-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6af68-147">Java</span><span class="sxs-lookup"><span data-stu-id="6af68-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6af68-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af68-148">Response</span></span>

<span data-ttu-id="6af68-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6af68-149">The following is an example of the response.</span></span>

> <span data-ttu-id="6af68-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6af68-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


