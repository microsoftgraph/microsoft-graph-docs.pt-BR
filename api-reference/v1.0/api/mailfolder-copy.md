---
title: 'mailFolder: copy'
description: Copie uma mailFolder e seu conteúdo para outra mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3a9f9b4a477619b159c7b9660674f1c7f75064e3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326678"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="110c3-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="110c3-103">mailFolder: copy</span></span>

<span data-ttu-id="110c3-104">Copie uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="110c3-104">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="110c3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="110c3-105">Permissions</span></span>

<span data-ttu-id="110c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="110c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="110c3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="110c3-108">Permission type</span></span> | <span data-ttu-id="110c3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="110c3-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="110c3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="110c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="110c3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="110c3-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="110c3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="110c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="110c3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="110c3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="110c3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="110c3-114">Application</span></span> | <span data-ttu-id="110c3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="110c3-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="110c3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="110c3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="110c3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="110c3-117">Request headers</span></span>
| <span data-ttu-id="110c3-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="110c3-118">Header</span></span> | <span data-ttu-id="110c3-119">Valor</span><span class="sxs-lookup"><span data-stu-id="110c3-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="110c3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="110c3-120">Authorization</span></span> | <span data-ttu-id="110c3-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="110c3-121"></span></span> <span data-ttu-id="110c3-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="110c3-122">Required.</span></span> |
| <span data-ttu-id="110c3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="110c3-123">Content-Type</span></span> | <span data-ttu-id="110c3-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="110c3-124"></span></span> <span data-ttu-id="110c3-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="110c3-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="110c3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="110c3-126">Request body</span></span>

<span data-ttu-id="110c3-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="110c3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="110c3-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="110c3-128">Parameter</span></span> | <span data-ttu-id="110c3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="110c3-129">Type</span></span> | <span data-ttu-id="110c3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="110c3-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="110c3-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="110c3-131">destinationId</span></span>|<span data-ttu-id="110c3-132">String</span><span class="sxs-lookup"><span data-stu-id="110c3-132">String</span></span>|<span data-ttu-id="110c3-133">A ID da pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="110c3-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="110c3-134">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="110c3-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="110c3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="110c3-135">Response</span></span>

<span data-ttu-id="110c3-136">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="110c3-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="110c3-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="110c3-137">Example</span></span>

<span data-ttu-id="110c3-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="110c3-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="110c3-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="110c3-139">Request</span></span>
<span data-ttu-id="110c3-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="110c3-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="110c3-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="110c3-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="110c3-142">C#</span><span class="sxs-lookup"><span data-stu-id="110c3-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="110c3-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="110c3-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="110c3-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="110c3-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="110c3-145">Java</span><span class="sxs-lookup"><span data-stu-id="110c3-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="110c3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="110c3-146">Response</span></span>

<span data-ttu-id="110c3-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="110c3-147">Here is an example of the response.</span></span>

> <span data-ttu-id="110c3-148">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="110c3-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="110c3-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="110c3-149">All the properties will be returned from an actual call.</span></span>
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
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
