---
title: Criar pasta filho
description: Use essa API para criar um novo mailFolder filho.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 312d26d32b49c9ccc14e6f83a4c1cb6392cdd8b5
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629172"
---
# <a name="create-child-folder"></a><span data-ttu-id="5aa22-103">Criar pasta filho</span><span class="sxs-lookup"><span data-stu-id="5aa22-103">Create child folder</span></span>

<span data-ttu-id="5aa22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aa22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aa22-105">Use essa API para criar um novo [mailFolder filho.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="5aa22-105">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="5aa22-106">Se você pretende que uma nova pasta seja oculta, você deve definir a **propriedade isHidden** como `true` na criação.</span><span class="sxs-lookup"><span data-stu-id="5aa22-106">If you intend a new folder to be hidden, you must set the **isHidden** property to `true` on creation.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aa22-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5aa22-107">Permissions</span></span>

<span data-ttu-id="5aa22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aa22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5aa22-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5aa22-110">Permission type</span></span> | <span data-ttu-id="5aa22-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5aa22-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="5aa22-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5aa22-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5aa22-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5aa22-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5aa22-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5aa22-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aa22-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5aa22-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5aa22-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5aa22-116">Application</span></span> | <span data-ttu-id="5aa22-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5aa22-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5aa22-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5aa22-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="5aa22-119">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="5aa22-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="5aa22-120">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5aa22-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5aa22-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5aa22-121">Request headers</span></span>

| <span data-ttu-id="5aa22-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5aa22-122">Header</span></span> | <span data-ttu-id="5aa22-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5aa22-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="5aa22-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5aa22-124">Authorization</span></span> | <span data-ttu-id="5aa22-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="5aa22-125">`Bearer {token}`.</span></span> <span data-ttu-id="5aa22-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aa22-126">Required.</span></span> |
| <span data-ttu-id="5aa22-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5aa22-127">Content-Type</span></span> | <span data-ttu-id="5aa22-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="5aa22-128">`application/json`.</span></span> <span data-ttu-id="5aa22-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aa22-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5aa22-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5aa22-130">Request body</span></span>

<span data-ttu-id="5aa22-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aa22-131">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="5aa22-132">**displayName** e **isHidden** são a única propriedade writable para um [objeto MailFolder.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="5aa22-132">**displayName** and **isHidden** are the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="5aa22-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5aa22-133">Parameter</span></span> | <span data-ttu-id="5aa22-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="5aa22-134">Type</span></span> | <span data-ttu-id="5aa22-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aa22-135">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="5aa22-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5aa22-136">displayName</span></span>|<span data-ttu-id="5aa22-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5aa22-137">String</span></span>|<span data-ttu-id="5aa22-138">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="5aa22-138">The display name of the new folder.</span></span>|
|<span data-ttu-id="5aa22-139">isHidden</span><span class="sxs-lookup"><span data-stu-id="5aa22-139">isHidden</span></span>|<span data-ttu-id="5aa22-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="5aa22-140">Boolean</span></span>|<span data-ttu-id="5aa22-141">Indica se a nova pasta está oculta.</span><span class="sxs-lookup"><span data-stu-id="5aa22-141">Indicates whether the new folder is hidden.</span></span> <span data-ttu-id="5aa22-142">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="5aa22-142">The default value is `false`.</span></span> <span data-ttu-id="5aa22-143">A configuração da propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="5aa22-143">Setting the property is optional.</span></span> <span data-ttu-id="5aa22-144">Depois de definido, você não pode atualizar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="5aa22-144">Once set, you cannot update this property.</span></span> <span data-ttu-id="5aa22-145">Confira mais informações em [Pastas de email ocultas](../resources/mailfolder.md#hidden-mail-folders)</span><span class="sxs-lookup"><span data-stu-id="5aa22-145">See more information in [Hidden mail folders](../resources/mailfolder.md#hidden-mail-folders)</span></span>|

## <a name="response"></a><span data-ttu-id="5aa22-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aa22-146">Response</span></span>

<span data-ttu-id="5aa22-147">Se tiver êxito, este método retornará `201 Created` o código de resposta e um objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aa22-147">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aa22-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5aa22-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5aa22-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5aa22-149">Request</span></span>

<span data-ttu-id="5aa22-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aa22-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5aa22-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aa22-151">HTTP</span></span>](#tab/http)
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
  "isHidden": true
}
```
# <a name="c"></a>[<span data-ttu-id="5aa22-152">C#</span><span class="sxs-lookup"><span data-stu-id="5aa22-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aa22-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aa22-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aa22-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aa22-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5aa22-155">Java</span><span class="sxs-lookup"><span data-stu-id="5aa22-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5aa22-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aa22-156">Response</span></span>

<span data-ttu-id="5aa22-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5aa22-157">The following is an example of the response.</span></span>

> <span data-ttu-id="5aa22-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5aa22-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "id-value",
  "isHidden": true
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


