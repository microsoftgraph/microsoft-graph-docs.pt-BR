---
title: Criar contato
description: Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d86f100f3343ffba2b3302927129bdd7a575329
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451704"
---
# <a name="create-contact"></a><span data-ttu-id="fe55e-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="fe55e-103">Create Contact</span></span>

<span data-ttu-id="fe55e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fe55e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe55e-105">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="fe55e-105">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe55e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe55e-106">Permissions</span></span>
<span data-ttu-id="fe55e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe55e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe55e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe55e-109">Permission type</span></span>      | <span data-ttu-id="fe55e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe55e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe55e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe55e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fe55e-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe55e-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fe55e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe55e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe55e-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe55e-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fe55e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe55e-115">Application</span></span> | <span data-ttu-id="fe55e-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe55e-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe55e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe55e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="fe55e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe55e-118">Request headers</span></span>
| <span data-ttu-id="fe55e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe55e-119">Header</span></span>       | <span data-ttu-id="fe55e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fe55e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe55e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe55e-121">Authorization</span></span>  | <span data-ttu-id="fe55e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe55e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fe55e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe55e-124">Content-Type</span></span>  | <span data-ttu-id="fe55e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe55e-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe55e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe55e-126">Request body</span></span>
<span data-ttu-id="fe55e-127">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="fe55e-127">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fe55e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe55e-128">Response</span></span>

<span data-ttu-id="fe55e-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe55e-129">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe55e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe55e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe55e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe55e-131">Request</span></span>
<span data-ttu-id="fe55e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe55e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fe55e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe55e-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fe55e-134">C#</span><span class="sxs-lookup"><span data-stu-id="fe55e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe55e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe55e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe55e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe55e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fe55e-137">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="fe55e-137">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="fe55e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe55e-138">Response</span></span>
<span data-ttu-id="fe55e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe55e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fe55e-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="fe55e-142">See also</span></span>

- [<span data-ttu-id="fe55e-143">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="fe55e-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fe55e-144">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="fe55e-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
