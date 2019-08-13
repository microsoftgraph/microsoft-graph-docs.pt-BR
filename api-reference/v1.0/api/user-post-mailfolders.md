---
title: Criar MailFolder
description: Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ecbfa56d17d73d288171baa59556380866272b98
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374376"
---
# <a name="create-mailfolder"></a><span data-ttu-id="dca77-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="dca77-103">Create MailFolder</span></span>

<span data-ttu-id="dca77-104">Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="dca77-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="dca77-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dca77-105">Permissions</span></span>
<span data-ttu-id="dca77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dca77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dca77-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dca77-108">Permission type</span></span>      | <span data-ttu-id="dca77-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dca77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dca77-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dca77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dca77-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca77-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dca77-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dca77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dca77-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca77-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dca77-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dca77-114">Application</span></span> | <span data-ttu-id="dca77-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca77-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dca77-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dca77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="dca77-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dca77-117">Request headers</span></span>
| <span data-ttu-id="dca77-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dca77-118">Header</span></span>       | <span data-ttu-id="dca77-119">Valor</span><span class="sxs-lookup"><span data-stu-id="dca77-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dca77-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="dca77-120">Authorization</span></span>  | <span data-ttu-id="dca77-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dca77-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dca77-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dca77-123">Content-Type</span></span>  | <span data-ttu-id="dca77-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dca77-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dca77-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dca77-125">Request body</span></span>
<span data-ttu-id="dca77-p103">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="dca77-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="dca77-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dca77-128">Parameter</span></span>    | <span data-ttu-id="dca77-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="dca77-129">Type</span></span>   |<span data-ttu-id="dca77-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="dca77-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dca77-131">displayName</span><span class="sxs-lookup"><span data-stu-id="dca77-131">displayName</span></span>|<span data-ttu-id="dca77-132">String</span><span class="sxs-lookup"><span data-stu-id="dca77-132">String</span></span>|<span data-ttu-id="dca77-133">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="dca77-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="dca77-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dca77-134">Response</span></span>

<span data-ttu-id="dca77-135">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dca77-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dca77-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dca77-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dca77-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dca77-137">Request</span></span>
<span data-ttu-id="dca77-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dca77-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dca77-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="dca77-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="dca77-140">C#</span><span class="sxs-lookup"><span data-stu-id="dca77-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dca77-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dca77-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dca77-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dca77-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dca77-143">Java</span><span class="sxs-lookup"><span data-stu-id="dca77-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dca77-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dca77-144">Response</span></span>
<span data-ttu-id="dca77-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dca77-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
