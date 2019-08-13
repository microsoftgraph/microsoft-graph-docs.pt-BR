---
title: Criar contato
description: Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cd18a66f4526d42e310af911e7e7f3a246cdfcfb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372619"
---
# <a name="create-contact"></a><span data-ttu-id="19550-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="19550-103">Create contact</span></span>

<span data-ttu-id="19550-104">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="19550-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="19550-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="19550-105">Permissions</span></span>

<span data-ttu-id="19550-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19550-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19550-108">Permission type</span></span>      | <span data-ttu-id="19550-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19550-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19550-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19550-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19550-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19550-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="19550-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19550-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19550-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19550-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="19550-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19550-114">Application</span></span> | <span data-ttu-id="19550-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19550-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="19550-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19550-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="19550-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19550-117">Request headers</span></span>

| <span data-ttu-id="19550-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19550-118">Header</span></span>       | <span data-ttu-id="19550-119">Valor</span><span class="sxs-lookup"><span data-stu-id="19550-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="19550-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="19550-120">Authorization</span></span>  | <span data-ttu-id="19550-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19550-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="19550-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19550-123">Content-Type</span></span>  | <span data-ttu-id="19550-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19550-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19550-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19550-126">Request body</span></span>
<span data-ttu-id="19550-127">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="19550-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="19550-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="19550-128">Response</span></span>

<span data-ttu-id="19550-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19550-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19550-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19550-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="19550-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19550-131">Request</span></span>

<span data-ttu-id="19550-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19550-132">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="19550-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="19550-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="19550-134">C#</span><span class="sxs-lookup"><span data-stu-id="19550-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19550-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19550-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19550-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="19550-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19550-137">Java</span><span class="sxs-lookup"><span data-stu-id="19550-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

<span data-ttu-id="19550-138">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="19550-138">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="19550-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="19550-139">Response</span></span>

<span data-ttu-id="19550-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19550-140">Here is an example of the response.</span></span> <span data-ttu-id="19550-141">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="19550-141">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="19550-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19550-142">All the properties will be returned from an actual call.</span></span>

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
