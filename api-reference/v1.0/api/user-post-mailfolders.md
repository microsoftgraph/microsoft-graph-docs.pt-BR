---
title: Criar MailFolder
description: Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 12ab9e5e491567a7b2d0bae60a209ed115828330
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278733"
---
# <a name="create-mailfolder"></a><span data-ttu-id="8673d-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="8673d-103">Create MailFolder</span></span>

<span data-ttu-id="8673d-104">Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8673d-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="8673d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8673d-105">Permissions</span></span>
<span data-ttu-id="8673d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8673d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8673d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8673d-108">Permission type</span></span>      | <span data-ttu-id="8673d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8673d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8673d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8673d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8673d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8673d-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8673d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8673d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8673d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8673d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8673d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8673d-114">Application</span></span> | <span data-ttu-id="8673d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8673d-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8673d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8673d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="8673d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8673d-117">Request headers</span></span>
| <span data-ttu-id="8673d-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8673d-118">Header</span></span>       | <span data-ttu-id="8673d-119">Valor</span><span class="sxs-lookup"><span data-stu-id="8673d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8673d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8673d-120">Authorization</span></span>  | <span data-ttu-id="8673d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8673d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8673d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8673d-123">Content-Type</span></span>  | <span data-ttu-id="8673d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8673d-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8673d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8673d-125">Request body</span></span>
<span data-ttu-id="8673d-p103">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="8673d-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="8673d-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8673d-128">Parameter</span></span>    | <span data-ttu-id="8673d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8673d-129">Type</span></span>   |<span data-ttu-id="8673d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8673d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8673d-131">displayName</span><span class="sxs-lookup"><span data-stu-id="8673d-131">displayName</span></span>|<span data-ttu-id="8673d-132">String</span><span class="sxs-lookup"><span data-stu-id="8673d-132">String</span></span>|<span data-ttu-id="8673d-133">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="8673d-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="8673d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8673d-134">Response</span></span>

<span data-ttu-id="8673d-135">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8673d-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8673d-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8673d-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8673d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8673d-137">Request</span></span>
<span data-ttu-id="8673d-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8673d-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="8673d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8673d-139">Response</span></span>
<span data-ttu-id="8673d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8673d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8673d-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8673d-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8673d-144">C#</span><span class="sxs-lookup"><span data-stu-id="8673d-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8673d-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="8673d-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8673d-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8673d-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_user-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/user-post-mailfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-post-mailfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-mailfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
