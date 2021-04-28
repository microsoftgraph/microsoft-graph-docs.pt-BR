---
title: Criar contato
description: Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cf20b2b9388dea809214e5978737c098892812b0
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061865"
---
# <a name="create-contact"></a><span data-ttu-id="cd15b-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="cd15b-103">Create contact</span></span>

<span data-ttu-id="cd15b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd15b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd15b-105">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="cd15b-105">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd15b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd15b-106">Permissions</span></span>

<span data-ttu-id="cd15b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd15b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd15b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd15b-109">Permission type</span></span>      | <span data-ttu-id="cd15b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd15b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd15b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd15b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd15b-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd15b-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cd15b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd15b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd15b-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd15b-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cd15b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd15b-115">Application</span></span> | <span data-ttu-id="cd15b-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd15b-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd15b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd15b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="cd15b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd15b-118">Request headers</span></span>

| <span data-ttu-id="cd15b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd15b-119">Header</span></span>       | <span data-ttu-id="cd15b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cd15b-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd15b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd15b-121">Authorization</span></span>  | <span data-ttu-id="cd15b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd15b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd15b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd15b-124">Content-Type</span></span>  | <span data-ttu-id="cd15b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd15b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd15b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd15b-127">Request body</span></span>
<span data-ttu-id="cd15b-128">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="cd15b-128">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cd15b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd15b-129">Response</span></span>

<span data-ttu-id="cd15b-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd15b-130">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd15b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd15b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd15b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd15b-132">Request</span></span>

<span data-ttu-id="cd15b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd15b-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cd15b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd15b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
# <a name="c"></a>[<span data-ttu-id="cd15b-135">C#</span><span class="sxs-lookup"><span data-stu-id="cd15b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd15b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd15b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd15b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd15b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd15b-138">Java</span><span class="sxs-lookup"><span data-stu-id="cd15b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

<span data-ttu-id="cd15b-139">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="cd15b-139">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="cd15b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd15b-140">Response</span></span>

<span data-ttu-id="cd15b-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd15b-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="cd15b-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cd15b-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

