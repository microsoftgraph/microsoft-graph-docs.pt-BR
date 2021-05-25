---
title: Criar MailFolder
description: Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a60f7166337933a3ee8897f9817c6adb148bd05c
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629396"
---
# <a name="create-mailfolder"></a><span data-ttu-id="887e6-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="887e6-103">Create MailFolder</span></span>

<span data-ttu-id="887e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="887e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="887e6-105">Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="887e6-105">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>

<span data-ttu-id="887e6-106">Se você pretende que uma nova pasta seja oculta, você deve definir a **propriedade isHidden** como `true` na criação.</span><span class="sxs-lookup"><span data-stu-id="887e6-106">If you intend a new folder to be hidden, you must set the **isHidden** property to `true` on creation.</span></span>

## <a name="permissions"></a><span data-ttu-id="887e6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="887e6-107">Permissions</span></span>
<span data-ttu-id="887e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="887e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="887e6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="887e6-110">Permission type</span></span>      | <span data-ttu-id="887e6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="887e6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="887e6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="887e6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="887e6-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="887e6-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="887e6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="887e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="887e6-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="887e6-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="887e6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="887e6-116">Application</span></span> | <span data-ttu-id="887e6-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="887e6-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="887e6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="887e6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="887e6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="887e6-119">Request headers</span></span>
| <span data-ttu-id="887e6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="887e6-120">Header</span></span>       | <span data-ttu-id="887e6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="887e6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="887e6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="887e6-122">Authorization</span></span>  | <span data-ttu-id="887e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="887e6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="887e6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="887e6-125">Content-Type</span></span>  | <span data-ttu-id="887e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="887e6-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="887e6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="887e6-127">Request body</span></span>
<span data-ttu-id="887e6-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="887e6-128">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="887e6-129">**displayName** e **isHidden** são a única propriedade writable para um [objeto mailFolder.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="887e6-129">**displayName** and **isHidden** are the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="887e6-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="887e6-130">Parameter</span></span>    | <span data-ttu-id="887e6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="887e6-131">Type</span></span>   |<span data-ttu-id="887e6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="887e6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="887e6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="887e6-133">displayName</span></span>|<span data-ttu-id="887e6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="887e6-134">String</span></span>|<span data-ttu-id="887e6-135">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="887e6-135">The display name of the new folder.</span></span>|
|<span data-ttu-id="887e6-136">isHidden</span><span class="sxs-lookup"><span data-stu-id="887e6-136">isHidden</span></span>|<span data-ttu-id="887e6-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="887e6-137">Boolean</span></span>|<span data-ttu-id="887e6-138">Indica se a nova pasta está oculta.</span><span class="sxs-lookup"><span data-stu-id="887e6-138">Indicates whether the new folder is hidden.</span></span> <span data-ttu-id="887e6-139">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="887e6-139">The default value is `false`.</span></span> <span data-ttu-id="887e6-140">A configuração da propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="887e6-140">Setting the property is optional.</span></span> <span data-ttu-id="887e6-141">Depois de definido, você não pode atualizar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="887e6-141">Once set, you cannot update this property.</span></span> <span data-ttu-id="887e6-142">Confira mais informações em [Pastas de email ocultas](../resources/mailfolder.md#hidden-mail-folders)</span><span class="sxs-lookup"><span data-stu-id="887e6-142">See more information in [Hidden mail folders](../resources/mailfolder.md#hidden-mail-folders)</span></span>|

## <a name="response"></a><span data-ttu-id="887e6-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="887e6-143">Response</span></span>

<span data-ttu-id="887e6-144">Se tiver êxito, este método retornará `201 Created` o código de resposta e um objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="887e6-144">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="887e6-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="887e6-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="887e6-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="887e6-146">Request</span></span>
<span data-ttu-id="887e6-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="887e6-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="887e6-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="887e6-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "Clutter",
  "isHidden": true
}
```
# <a name="c"></a>[<span data-ttu-id="887e6-149">C#</span><span class="sxs-lookup"><span data-stu-id="887e6-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="887e6-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="887e6-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="887e6-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="887e6-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="887e6-152">Java</span><span class="sxs-lookup"><span data-stu-id="887e6-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="887e6-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="887e6-153">Response</span></span>
<span data-ttu-id="887e6-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="887e6-154">Here is an example of the response.</span></span> 

><span data-ttu-id="887e6-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="887e6-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "displayName": "Clutter",
  "parentFolderId": "AQMkADlmOGQwZmU3LWVjOWMtNDhiYgAtODcxNy1",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "hN2Y5OGRhNGYwODEALgAAA0DAKbvJvFhJgcT3lZpkhNQBAA1",
  "isHidden": true
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

