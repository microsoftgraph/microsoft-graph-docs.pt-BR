---
title: Criar contato
description: Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ab836089b926324b5163c12ab234f6bfc791abe8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086848"
---
# <a name="create-contact"></a><span data-ttu-id="4eb7b-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="4eb7b-103">Create Contact</span></span>

<span data-ttu-id="4eb7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eb7b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4eb7b-105">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="4eb7b-105">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4eb7b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4eb7b-106">Permissions</span></span>
<span data-ttu-id="4eb7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eb7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eb7b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4eb7b-109">Permission type</span></span>      | <span data-ttu-id="4eb7b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4eb7b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4eb7b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4eb7b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4eb7b-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eb7b-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4eb7b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4eb7b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eb7b-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eb7b-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4eb7b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4eb7b-115">Application</span></span> | <span data-ttu-id="4eb7b-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eb7b-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eb7b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4eb7b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="4eb7b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4eb7b-118">Request headers</span></span>
| <span data-ttu-id="4eb7b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4eb7b-119">Header</span></span>       | <span data-ttu-id="4eb7b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4eb7b-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4eb7b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4eb7b-121">Authorization</span></span>  | <span data-ttu-id="4eb7b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4eb7b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4eb7b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4eb7b-124">Content-Type</span></span>  | <span data-ttu-id="4eb7b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4eb7b-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4eb7b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4eb7b-126">Request body</span></span>
<span data-ttu-id="4eb7b-127">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="4eb7b-127">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4eb7b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4eb7b-128">Response</span></span>

<span data-ttu-id="4eb7b-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4eb7b-129">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eb7b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4eb7b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4eb7b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4eb7b-131">Request</span></span>
<span data-ttu-id="4eb7b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4eb7b-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4eb7b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4eb7b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky"
    }
  ],
  "businessPhones": [
    "+1 732 555 0102"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="4eb7b-134">C#</span><span class="sxs-lookup"><span data-stu-id="4eb7b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4eb7b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4eb7b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4eb7b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4eb7b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4eb7b-137">Java</span><span class="sxs-lookup"><span data-stu-id="4eb7b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4eb7b-138">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="4eb7b-138">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="4eb7b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4eb7b-139">Response</span></span>
<span data-ttu-id="4eb7b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4eb7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "createdDateTime": "2015-11-09T02:14:32Z",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z",
   "displayName": "Pavel Bansky"
}
```

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

