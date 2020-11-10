---
title: Criar contato
description: Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 63603ccc2feb93185bb73d28b0276c81d87d1d61
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964065"
---
# <a name="create-contact"></a><span data-ttu-id="730e3-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="730e3-103">Create Contact</span></span>

<span data-ttu-id="730e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="730e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="730e3-105">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="730e3-105">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="730e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="730e3-106">Permissions</span></span>
<span data-ttu-id="730e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="730e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="730e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="730e3-109">Permission type</span></span>      | <span data-ttu-id="730e3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="730e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="730e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="730e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="730e3-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="730e3-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="730e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="730e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="730e3-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="730e3-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="730e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="730e3-115">Application</span></span> | <span data-ttu-id="730e3-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="730e3-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="730e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="730e3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="730e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="730e3-118">Request headers</span></span>
| <span data-ttu-id="730e3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="730e3-119">Header</span></span>       | <span data-ttu-id="730e3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="730e3-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="730e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="730e3-121">Authorization</span></span>  | <span data-ttu-id="730e3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="730e3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="730e3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="730e3-124">Content-Type</span></span>  | <span data-ttu-id="730e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="730e3-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="730e3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="730e3-126">Request body</span></span>
<span data-ttu-id="730e3-127">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="730e3-127">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="730e3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="730e3-128">Response</span></span>

<span data-ttu-id="730e3-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="730e3-129">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="730e3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="730e3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="730e3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="730e3-131">Request</span></span>
<span data-ttu-id="730e3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="730e3-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="730e3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="730e3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@contoso.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "personal"
    },
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "other",
      "otherLabel": "Volunteer work"
    }
  ],
  "phones" : [
    {
      "number": "+1 732 555 0102",
      "type": "business"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="730e3-134">C#</span><span class="sxs-lookup"><span data-stu-id="730e3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="730e3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="730e3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="730e3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="730e3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="730e3-137">Java</span><span class="sxs-lookup"><span data-stu-id="730e3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="730e3-138">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="730e3-138">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="730e3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="730e3-139">Response</span></span>
<span data-ttu-id="730e3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="730e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T19:56:07Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@contoso.onmicrosoft.com"
        },
        {
            "otherLabel": "Volunteer work",
            "type":"other",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="730e3-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="730e3-143">See also</span></span>

- [<span data-ttu-id="730e3-144">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="730e3-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="730e3-145">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="730e3-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

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


