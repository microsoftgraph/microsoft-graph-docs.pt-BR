---
title: Criar contato
description: Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.
author: dkershaw10
ms.openlocfilehash: cb95f9affa637dfb04109fc7192c6ddafe61362a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318988"
---
# <a name="create-contact"></a><span data-ttu-id="4dc17-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="4dc17-103">Create Contact</span></span>

> <span data-ttu-id="4dc17-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4dc17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dc17-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4dc17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4dc17-106">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="4dc17-106">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4dc17-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4dc17-107">Permissions</span></span>
<span data-ttu-id="4dc17-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dc17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dc17-110">Permission type</span></span>      | <span data-ttu-id="4dc17-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4dc17-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dc17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dc17-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4dc17-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dc17-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4dc17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dc17-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dc17-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dc17-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4dc17-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dc17-116">Application</span></span> | <span data-ttu-id="4dc17-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dc17-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dc17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dc17-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="4dc17-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc17-119">Request headers</span></span>
| <span data-ttu-id="4dc17-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4dc17-120">Header</span></span>       | <span data-ttu-id="4dc17-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4dc17-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4dc17-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dc17-122">Authorization</span></span>  | <span data-ttu-id="4dc17-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dc17-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4dc17-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4dc17-125">Content-Type</span></span>  | <span data-ttu-id="4dc17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4dc17-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4dc17-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc17-127">Request body</span></span>
<span data-ttu-id="4dc17-128">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="4dc17-128">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4dc17-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dc17-129">Response</span></span>

<span data-ttu-id="4dc17-130">Se tiver êxito, este método retornará `201 Created` objeto response de código e [de contato](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dc17-130">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dc17-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dc17-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4dc17-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc17-132">Request</span></span>
<span data-ttu-id="4dc17-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dc17-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="4dc17-134">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="4dc17-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="4dc17-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dc17-135">Response</span></span>
<span data-ttu-id="4dc17-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dc17-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4dc17-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="4dc17-139">See also</span></span>

- [<span data-ttu-id="4dc17-140">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="4dc17-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4dc17-141">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="4dc17-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
