---
title: Criar contato
description: Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fabcaa698c21b4a0118ca108861ffde4b751374a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269955"
---
# <a name="create-contact"></a><span data-ttu-id="28b26-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="28b26-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28b26-104">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="28b26-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="28b26-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="28b26-105">Permissions</span></span>
<span data-ttu-id="28b26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28b26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28b26-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28b26-108">Permission type</span></span>      | <span data-ttu-id="28b26-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28b26-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28b26-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28b26-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28b26-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28b26-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="28b26-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28b26-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28b26-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28b26-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="28b26-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28b26-114">Application</span></span> | <span data-ttu-id="28b26-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28b26-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="28b26-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28b26-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="28b26-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28b26-117">Request headers</span></span>
| <span data-ttu-id="28b26-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28b26-118">Header</span></span>       | <span data-ttu-id="28b26-119">Valor</span><span class="sxs-lookup"><span data-stu-id="28b26-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28b26-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="28b26-120">Authorization</span></span>  | <span data-ttu-id="28b26-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28b26-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="28b26-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28b26-123">Content-Type</span></span>  | <span data-ttu-id="28b26-124">application/json</span><span class="sxs-lookup"><span data-stu-id="28b26-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28b26-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28b26-125">Request body</span></span>
<span data-ttu-id="28b26-126">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="28b26-126">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="28b26-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b26-127">Response</span></span>

<span data-ttu-id="28b26-128">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28b26-128">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28b26-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28b26-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28b26-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b26-130">Request</span></span>
<span data-ttu-id="28b26-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28b26-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="28b26-132">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="28b26-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="28b26-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b26-133">Response</span></span>
<span data-ttu-id="28b26-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28b26-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="28b26-137">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="28b26-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="28b26-138">C#</span><span class="sxs-lookup"><span data-stu-id="28b26-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28b26-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="28b26-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="28b26-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="28b26-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="28b26-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="28b26-141">See also</span></span>

- [<span data-ttu-id="28b26-142">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="28b26-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="28b26-143">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="28b26-143">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
