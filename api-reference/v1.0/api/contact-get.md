---
title: Obter contato
description: Recupere as propriedades e os relacionamentos do objeto contact.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 057a97ba25d12f7baaa951ba7750cdd4ab9dd435
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860904"
---
# <a name="get-contact"></a><span data-ttu-id="93510-103">Obter contato</span><span class="sxs-lookup"><span data-stu-id="93510-103">Get contact</span></span>

<span data-ttu-id="93510-104">Recupere as propriedades e os relacionamentos do objeto contact.</span><span class="sxs-lookup"><span data-stu-id="93510-104">Retrieve the properties and relationships of a contact object.</span></span>

<span data-ttu-id="93510-105">Há dois cenários em que um aplicativo pode receber um contato na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="93510-105">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="93510-106">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="93510-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="93510-107">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de contato com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="93510-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="93510-108">Consulte os [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="93510-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="93510-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="93510-109">Permissions</span></span>
<span data-ttu-id="93510-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93510-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93510-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93510-112">Permission type</span></span>      | <span data-ttu-id="93510-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93510-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93510-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93510-114">Delegated (work or school account)</span></span> | <span data-ttu-id="93510-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93510-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="93510-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93510-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93510-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93510-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="93510-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93510-118">Application</span></span> | <span data-ttu-id="93510-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93510-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="93510-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93510-120">HTTP request</span></span>
<span data-ttu-id="93510-121"><!-- { "blockType": "ignored" } -->Um [contato](../resources/contact.md) do padrão de um usuário [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="93510-121"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="93510-122">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="93510-122">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="93510-p103">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="93510-p103">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93510-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="93510-125">Optional query parameters</span></span>
|<span data-ttu-id="93510-126">Nome</span><span class="sxs-lookup"><span data-stu-id="93510-126">Name</span></span>|<span data-ttu-id="93510-127">Valor</span><span class="sxs-lookup"><span data-stu-id="93510-127">Value</span></span>|<span data-ttu-id="93510-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="93510-128">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="93510-129">$expand</span><span class="sxs-lookup"><span data-stu-id="93510-129">$expand</span></span>|<span data-ttu-id="93510-130">string</span><span class="sxs-lookup"><span data-stu-id="93510-130">string</span></span>|<span data-ttu-id="93510-p104">Lista separada por vírgulas de relações para expandir e incluir na resposta. Consulte a tabela de relacionamentos do objeto [contact](../resources/contact.md) para conhecer os nomes compatíveis.</span><span class="sxs-lookup"><span data-stu-id="93510-p104">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="93510-133">$select</span><span class="sxs-lookup"><span data-stu-id="93510-133">$select</span></span>|<span data-ttu-id="93510-134">string</span><span class="sxs-lookup"><span data-stu-id="93510-134">string</span></span>|<span data-ttu-id="93510-135">Lista separada por vírgulas de propriedades para incluir na resposta.</span><span class="sxs-lookup"><span data-stu-id="93510-135">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="93510-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93510-136">Request headers</span></span>
| <span data-ttu-id="93510-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93510-137">Header</span></span>       | <span data-ttu-id="93510-138">Valor</span><span class="sxs-lookup"><span data-stu-id="93510-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93510-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="93510-139">Authorization</span></span>  | <span data-ttu-id="93510-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93510-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93510-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93510-142">Request body</span></span>
<span data-ttu-id="93510-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93510-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93510-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="93510-144">Response</span></span>

<span data-ttu-id="93510-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93510-145">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93510-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93510-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93510-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93510-147">Request</span></span>
<span data-ttu-id="93510-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93510-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="93510-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="93510-149">Response</span></span>
<span data-ttu-id="93510-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93510-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "https://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {},
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
