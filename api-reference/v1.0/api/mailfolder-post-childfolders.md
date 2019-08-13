---
title: Criar MailFolder
description: Use essa API para criar uma nova mailfolder filha.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2ff43d14003fd77e18817af77f5718e2eab8589b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374943"
---
# <a name="create-mailfolder"></a><span data-ttu-id="9eb77-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="9eb77-103">Create MailFolder</span></span>

<span data-ttu-id="9eb77-104">Use essa API para criar uma nova mailfolder filha.</span><span class="sxs-lookup"><span data-stu-id="9eb77-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9eb77-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9eb77-105">Permissions</span></span>

<span data-ttu-id="9eb77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9eb77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9eb77-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9eb77-108">Permission type</span></span> | <span data-ttu-id="9eb77-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9eb77-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="9eb77-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9eb77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9eb77-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9eb77-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9eb77-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9eb77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eb77-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9eb77-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9eb77-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9eb77-114">Application</span></span> | <span data-ttu-id="9eb77-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9eb77-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9eb77-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9eb77-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="9eb77-117">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="9eb77-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="9eb77-118">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9eb77-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9eb77-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9eb77-119">Request headers</span></span>

| <span data-ttu-id="9eb77-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9eb77-120">Header</span></span> | <span data-ttu-id="9eb77-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9eb77-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="9eb77-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9eb77-122">Authorization</span></span> | <span data-ttu-id="9eb77-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="9eb77-123"></span></span> <span data-ttu-id="9eb77-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9eb77-124">Required.</span></span> |
| <span data-ttu-id="9eb77-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9eb77-125">Content-Type</span></span> | <span data-ttu-id="9eb77-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="9eb77-126"></span></span> <span data-ttu-id="9eb77-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9eb77-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9eb77-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9eb77-128">Request body</span></span>

<span data-ttu-id="9eb77-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9eb77-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="9eb77-130">**DisplayName** é a única propriedade gravável para um objeto [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="9eb77-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="9eb77-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9eb77-131">Parameter</span></span> | <span data-ttu-id="9eb77-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9eb77-132">Type</span></span> | <span data-ttu-id="9eb77-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9eb77-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="9eb77-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9eb77-134">displayName</span></span>|<span data-ttu-id="9eb77-135">String</span><span class="sxs-lookup"><span data-stu-id="9eb77-135">String</span></span>|<span data-ttu-id="9eb77-136">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="9eb77-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="9eb77-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eb77-137">Response</span></span>

<span data-ttu-id="9eb77-138">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9eb77-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eb77-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9eb77-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9eb77-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9eb77-140">Request</span></span>

<span data-ttu-id="9eb77-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9eb77-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9eb77-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9eb77-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9eb77-143">C#</span><span class="sxs-lookup"><span data-stu-id="9eb77-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9eb77-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9eb77-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9eb77-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9eb77-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9eb77-146">Java</span><span class="sxs-lookup"><span data-stu-id="9eb77-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9eb77-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eb77-147">Response</span></span>
<span data-ttu-id="9eb77-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9eb77-148">Here is an example of the response.</span></span>

> <span data-ttu-id="9eb77-149">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9eb77-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9eb77-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9eb77-150">All the properties will be returned from an actual call.</span></span>
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
