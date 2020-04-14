---
title: Excluir contato
description: Exclua o contato.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 909e0d8e3b0e3e811035db29c071c476b562487a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382081"
---
# <a name="delete-contact"></a><span data-ttu-id="d68d3-103">Excluir contato</span><span class="sxs-lookup"><span data-stu-id="d68d3-103">Delete contact</span></span>

<span data-ttu-id="d68d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d68d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d68d3-105">Exclua o contato.</span><span class="sxs-lookup"><span data-stu-id="d68d3-105">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="d68d3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d68d3-106">Permissions</span></span>
<span data-ttu-id="d68d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d68d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d68d3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d68d3-109">Permission type</span></span>      | <span data-ttu-id="d68d3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d68d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d68d3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d68d3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d68d3-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d68d3-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d68d3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d68d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d68d3-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d68d3-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d68d3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d68d3-115">Application</span></span> | <span data-ttu-id="d68d3-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d68d3-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d68d3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d68d3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d68d3-118">Um [contato](../resources/contact.md) do [contactFolder](../resources/contactfolder.md)padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="d68d3-118">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="d68d3-119">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="d68d3-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="d68d3-120">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="d68d3-120">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="d68d3-121">O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="d68d3-121">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d68d3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d68d3-122">Request headers</span></span>
| <span data-ttu-id="d68d3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d68d3-123">Header</span></span>       | <span data-ttu-id="d68d3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d68d3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d68d3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d68d3-125">Authorization</span></span>  | <span data-ttu-id="d68d3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d68d3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d68d3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d68d3-128">Request body</span></span>
<span data-ttu-id="d68d3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d68d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d68d3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d68d3-130">Response</span></span>

<span data-ttu-id="d68d3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d68d3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d68d3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d68d3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d68d3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d68d3-134">Request</span></span>
<span data-ttu-id="d68d3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d68d3-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d68d3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d68d3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="d68d3-137">C#</span><span class="sxs-lookup"><span data-stu-id="d68d3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d68d3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d68d3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d68d3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d68d3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d68d3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d68d3-140">Response</span></span>
<span data-ttu-id="d68d3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d68d3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
