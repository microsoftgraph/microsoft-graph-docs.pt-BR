---
title: Excluir contato
description: Exclui um contato.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e483fd624baf0ec0f534b7435737fb59e6fc10f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003277"
---
# <a name="delete-contact"></a><span data-ttu-id="baf18-103">Excluir contato</span><span class="sxs-lookup"><span data-stu-id="baf18-103">Delete contact</span></span>

<span data-ttu-id="baf18-104">Exclui um contato.</span><span class="sxs-lookup"><span data-stu-id="baf18-104">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="baf18-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="baf18-105">Permissions</span></span>
<span data-ttu-id="baf18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baf18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baf18-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="baf18-108">Permission type</span></span>      | <span data-ttu-id="baf18-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="baf18-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baf18-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="baf18-110">Delegated (work or school account)</span></span> | <span data-ttu-id="baf18-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baf18-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="baf18-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="baf18-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baf18-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baf18-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="baf18-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="baf18-114">Application</span></span> | <span data-ttu-id="baf18-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baf18-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="baf18-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="baf18-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="baf18-117">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="baf18-117">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="baf18-118">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="baf18-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="baf18-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="baf18-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="baf18-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="baf18-121">Request headers</span></span>
| <span data-ttu-id="baf18-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="baf18-122">Header</span></span>       | <span data-ttu-id="baf18-123">Valor</span><span class="sxs-lookup"><span data-stu-id="baf18-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="baf18-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="baf18-124">Authorization</span></span>  | <span data-ttu-id="baf18-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="baf18-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="baf18-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="baf18-127">Request body</span></span>
<span data-ttu-id="baf18-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="baf18-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baf18-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="baf18-129">Response</span></span>

<span data-ttu-id="baf18-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="baf18-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baf18-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="baf18-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="baf18-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="baf18-133">Request</span></span>
<span data-ttu-id="baf18-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="baf18-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="baf18-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="baf18-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="baf18-136">C#</span><span class="sxs-lookup"><span data-stu-id="baf18-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="baf18-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="baf18-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="baf18-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="baf18-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="baf18-139">Java</span><span class="sxs-lookup"><span data-stu-id="baf18-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="baf18-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="baf18-140">Response</span></span>
<span data-ttu-id="baf18-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="baf18-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
