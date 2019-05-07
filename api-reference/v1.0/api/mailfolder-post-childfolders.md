---
title: Criar MailFolder
description: Use essa API para criar uma nova mailfolder filha.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 872e54f53fbc79ee3f3e015d1f50f4ef3288cd29
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612220"
---
# <a name="create-mailfolder"></a><span data-ttu-id="5c902-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="5c902-103">Create MailFolder</span></span>

<span data-ttu-id="5c902-104">Use essa API para criar uma nova mailfolder filha.</span><span class="sxs-lookup"><span data-stu-id="5c902-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c902-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c902-105">Permissions</span></span>

<span data-ttu-id="5c902-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c902-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c902-108">Permission type</span></span> | <span data-ttu-id="5c902-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c902-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="5c902-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c902-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c902-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c902-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5c902-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c902-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c902-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c902-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5c902-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c902-114">Application</span></span> | <span data-ttu-id="5c902-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c902-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c902-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c902-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="5c902-117">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="5c902-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="5c902-118">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5c902-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c902-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c902-119">Request headers</span></span>

| <span data-ttu-id="5c902-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c902-120">Header</span></span> | <span data-ttu-id="5c902-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5c902-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="5c902-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c902-122">Authorization</span></span> | <span data-ttu-id="5c902-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="5c902-123"></span></span> <span data-ttu-id="5c902-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c902-124">Required.</span></span> |
| <span data-ttu-id="5c902-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c902-125">Content-Type</span></span> | <span data-ttu-id="5c902-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="5c902-126"></span></span> <span data-ttu-id="5c902-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c902-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c902-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c902-128">Request body</span></span>

<span data-ttu-id="5c902-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c902-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="5c902-130">**DisplayName** é a única propriedade gravável para um objeto [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="5c902-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="5c902-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5c902-131">Parameter</span></span> | <span data-ttu-id="5c902-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c902-132">Type</span></span> | <span data-ttu-id="5c902-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c902-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="5c902-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5c902-134">displayName</span></span>|<span data-ttu-id="5c902-135">String</span><span class="sxs-lookup"><span data-stu-id="5c902-135">String</span></span>|<span data-ttu-id="5c902-136">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="5c902-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="5c902-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c902-137">Response</span></span>

<span data-ttu-id="5c902-138">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c902-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c902-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c902-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5c902-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c902-140">Request</span></span>

<span data-ttu-id="5c902-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c902-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5c902-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c902-142">Response</span></span>
<span data-ttu-id="5c902-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c902-143">Here is an example of the response.</span></span>

> <span data-ttu-id="5c902-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c902-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5c902-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c902-145">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5c902-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5c902-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5c902-147">Basic</span><span class="sxs-lookup"><span data-stu-id="5c902-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c902-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c902-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-post-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-post-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
