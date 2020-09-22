---
title: Criar MailFolder
description: Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5b8e6c41de41f23b5a8b3d6e1a31394773c666b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064539"
---
# <a name="create-mailfolder"></a><span data-ttu-id="37afa-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="37afa-103">Create MailFolder</span></span>

<span data-ttu-id="37afa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37afa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37afa-105">Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="37afa-105">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="37afa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37afa-106">Permissions</span></span>
<span data-ttu-id="37afa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37afa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37afa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37afa-109">Permission type</span></span>      | <span data-ttu-id="37afa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37afa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37afa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37afa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37afa-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37afa-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="37afa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37afa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37afa-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37afa-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="37afa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37afa-115">Application</span></span> | <span data-ttu-id="37afa-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37afa-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="37afa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37afa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="37afa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37afa-118">Request headers</span></span>
| <span data-ttu-id="37afa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37afa-119">Header</span></span>       | <span data-ttu-id="37afa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="37afa-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37afa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37afa-121">Authorization</span></span>  | <span data-ttu-id="37afa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37afa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="37afa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37afa-124">Content-Type</span></span>  | <span data-ttu-id="37afa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37afa-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37afa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37afa-126">Request body</span></span>
<span data-ttu-id="37afa-p103">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="37afa-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="37afa-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="37afa-129">Parameter</span></span>    | <span data-ttu-id="37afa-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="37afa-130">Type</span></span>   |<span data-ttu-id="37afa-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="37afa-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37afa-132">displayName</span><span class="sxs-lookup"><span data-stu-id="37afa-132">displayName</span></span>|<span data-ttu-id="37afa-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37afa-133">String</span></span>|<span data-ttu-id="37afa-134">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="37afa-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="37afa-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="37afa-135">Response</span></span>

<span data-ttu-id="37afa-136">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37afa-136">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37afa-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37afa-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37afa-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37afa-138">Request</span></span>
<span data-ttu-id="37afa-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37afa-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37afa-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="37afa-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="37afa-141">C#</span><span class="sxs-lookup"><span data-stu-id="37afa-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37afa-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37afa-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37afa-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37afa-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="37afa-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="37afa-144">Response</span></span>
<span data-ttu-id="37afa-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37afa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


