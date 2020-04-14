---
title: Criar contato
description: Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d0238dc7b065e7fd8be884c47cbcab8622df81bf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43360977"
---
# <a name="create-contact"></a><span data-ttu-id="533db-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="533db-103">Create Contact</span></span>

<span data-ttu-id="533db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="533db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="533db-105">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="533db-105">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="533db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="533db-106">Permissions</span></span>
<span data-ttu-id="533db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="533db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="533db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="533db-109">Permission type</span></span>      | <span data-ttu-id="533db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="533db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="533db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="533db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="533db-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="533db-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="533db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="533db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="533db-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="533db-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="533db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="533db-115">Application</span></span> | <span data-ttu-id="533db-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="533db-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="533db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="533db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="533db-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="533db-118">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="533db-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="533db-119">Request headers</span></span>
| <span data-ttu-id="533db-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="533db-120">Header</span></span>       | <span data-ttu-id="533db-121">Valor</span><span class="sxs-lookup"><span data-stu-id="533db-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="533db-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="533db-122">Authorization</span></span>  | <span data-ttu-id="533db-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="533db-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="533db-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="533db-125">Content-Type</span></span>  | <span data-ttu-id="533db-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="533db-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="533db-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="533db-128">Request body</span></span>
<span data-ttu-id="533db-129">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="533db-129">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="533db-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="533db-130">Response</span></span>

<span data-ttu-id="533db-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="533db-131">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="533db-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="533db-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="533db-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="533db-133">Request</span></span>
<span data-ttu-id="533db-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="533db-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="533db-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="533db-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
# <a name="c"></a>[<span data-ttu-id="533db-136">C#</span><span class="sxs-lookup"><span data-stu-id="533db-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="533db-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="533db-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="533db-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="533db-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="533db-139">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="533db-139">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="533db-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="533db-140">Response</span></span>
<span data-ttu-id="533db-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="533db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
