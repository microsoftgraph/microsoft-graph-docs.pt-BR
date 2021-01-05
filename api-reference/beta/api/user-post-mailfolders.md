---
title: Criar MailFolder
description: Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 07913741d015830d395c104c34786009703c8133
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754114"
---
# <a name="create-mailfolder"></a><span data-ttu-id="d3e10-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="d3e10-103">Create MailFolder</span></span>

<span data-ttu-id="d3e10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3e10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3e10-105">Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="d3e10-105">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>

<span data-ttu-id="d3e10-106">Se você pretende que uma nova pasta fique oculta, você deve definir a propriedade **IsHidden** como `true` on Creation.</span><span class="sxs-lookup"><span data-stu-id="d3e10-106">If you intend a new folder to be hidden, you must set the **isHidden** property to `true` on creation.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3e10-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3e10-107">Permissions</span></span>
<span data-ttu-id="d3e10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e10-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3e10-110">Permission type</span></span>      | <span data-ttu-id="d3e10-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3e10-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3e10-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3e10-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d3e10-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3e10-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d3e10-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3e10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3e10-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3e10-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d3e10-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3e10-116">Application</span></span> | <span data-ttu-id="d3e10-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3e10-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3e10-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e10-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="d3e10-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e10-119">Request headers</span></span>
| <span data-ttu-id="d3e10-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3e10-120">Header</span></span>       | <span data-ttu-id="d3e10-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d3e10-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3e10-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3e10-122">Authorization</span></span>  | <span data-ttu-id="d3e10-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3e10-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d3e10-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3e10-125">Content-Type</span></span>  | <span data-ttu-id="d3e10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3e10-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3e10-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e10-127">Request body</span></span>
<span data-ttu-id="d3e10-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3e10-128">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="d3e10-129">**DisplayName** e **IsHidden** são a única propriedade gravável para um objeto [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="d3e10-129">**displayName** and **isHidden** are the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="d3e10-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d3e10-130">Parameter</span></span>    | <span data-ttu-id="d3e10-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3e10-131">Type</span></span>   |<span data-ttu-id="d3e10-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3e10-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3e10-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d3e10-133">displayName</span></span>|<span data-ttu-id="d3e10-134">String</span><span class="sxs-lookup"><span data-stu-id="d3e10-134">String</span></span>|<span data-ttu-id="d3e10-135">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="d3e10-135">The display name of the new folder.</span></span>|
|<span data-ttu-id="d3e10-136">isHidden</span><span class="sxs-lookup"><span data-stu-id="d3e10-136">isHidden</span></span>|<span data-ttu-id="d3e10-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="d3e10-137">Boolean</span></span>|<span data-ttu-id="d3e10-138">Indica se a nova pasta está oculta.</span><span class="sxs-lookup"><span data-stu-id="d3e10-138">Indicates whether the new folder is hidden.</span></span> <span data-ttu-id="d3e10-139">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="d3e10-139">The default value is `false`.</span></span> <span data-ttu-id="d3e10-140">A definição da propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="d3e10-140">Setting the property is optional.</span></span> <span data-ttu-id="d3e10-141">Uma vez definido, você não pode atualizar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="d3e10-141">Once set, you cannot update this property.</span></span> <span data-ttu-id="d3e10-142">Confira mais informações em [pastas de email ocultas](../resources/mailfolder.md#hidden-mail-folders)</span><span class="sxs-lookup"><span data-stu-id="d3e10-142">See more information in [Hidden mail folders](../resources/mailfolder.md#hidden-mail-folders)</span></span>|

## <a name="response"></a><span data-ttu-id="d3e10-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e10-143">Response</span></span>

<span data-ttu-id="d3e10-144">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3e10-144">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e10-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3e10-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3e10-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e10-146">Request</span></span>
<span data-ttu-id="d3e10-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3e10-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3e10-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e10-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "Clutter",
  "isHidden": true
}
```
# <a name="c"></a>[<span data-ttu-id="d3e10-149">C#</span><span class="sxs-lookup"><span data-stu-id="d3e10-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3e10-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3e10-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3e10-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3e10-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3e10-152">Java</span><span class="sxs-lookup"><span data-stu-id="d3e10-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3e10-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e10-153">Response</span></span>
<span data-ttu-id="d3e10-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3e10-154">Here is an example of the response.</span></span> 

><span data-ttu-id="d3e10-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d3e10-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "hN2Y5OGRhNGYwODEALgAAA0DAKbvJvFhJgcT3lZpkhNQBAA1",
  "displayName": "Clutter",
  "parentFolderId": "AQMkADlmOGQwZmU3LWVjOWMtNDhiYgAtODcxNy1",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "wellKnownName": null,
  "isHidden": true
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


