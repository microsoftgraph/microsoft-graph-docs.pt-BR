---
title: Excluir contato
description: Excluir contato.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4404b6b7137d7526d8352b2807cff0c0add7b27c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472542"
---
# <a name="delete-contact"></a><span data-ttu-id="db0f0-103">Excluir contato</span><span class="sxs-lookup"><span data-stu-id="db0f0-103">Delete contact</span></span>

<span data-ttu-id="db0f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db0f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db0f0-105">Excluir contato.</span><span class="sxs-lookup"><span data-stu-id="db0f0-105">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="db0f0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="db0f0-106">Permissions</span></span>
<span data-ttu-id="db0f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db0f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db0f0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db0f0-109">Permission type</span></span>      | <span data-ttu-id="db0f0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db0f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db0f0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db0f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db0f0-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db0f0-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="db0f0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db0f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db0f0-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db0f0-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="db0f0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db0f0-115">Application</span></span> | <span data-ttu-id="db0f0-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db0f0-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="db0f0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db0f0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="db0f0-118">Um [contato](../resources/contact.md) do [contactFolder](../resources/contactfolder.md)padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="db0f0-118">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="db0f0-119">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="db0f0-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="db0f0-120">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="db0f0-120">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="db0f0-121">O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="db0f0-121">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="db0f0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db0f0-122">Request headers</span></span>
| <span data-ttu-id="db0f0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db0f0-123">Header</span></span>       | <span data-ttu-id="db0f0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="db0f0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db0f0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="db0f0-125">Authorization</span></span>  | <span data-ttu-id="db0f0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db0f0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db0f0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db0f0-128">Request body</span></span>
<span data-ttu-id="db0f0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db0f0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db0f0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="db0f0-130">Response</span></span>

<span data-ttu-id="db0f0-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db0f0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db0f0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db0f0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db0f0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db0f0-134">Request</span></span>
<span data-ttu-id="db0f0-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db0f0-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db0f0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="db0f0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="db0f0-137">C#</span><span class="sxs-lookup"><span data-stu-id="db0f0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db0f0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db0f0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db0f0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db0f0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db0f0-140">Java</span><span class="sxs-lookup"><span data-stu-id="db0f0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db0f0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="db0f0-141">Response</span></span>
<span data-ttu-id="db0f0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db0f0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


