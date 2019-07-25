---
title: Obter contato
description: Recupere as propriedades e os relacionamentos do objeto contact.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2f5b146d6fa47ed643a4ac1dc1a4a2e2650dcc8b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885133"
---
# <a name="get-contact"></a><span data-ttu-id="2d739-103">Obter contato</span><span class="sxs-lookup"><span data-stu-id="2d739-103">Get contact</span></span>

<span data-ttu-id="2d739-104">Recupere as propriedades e os relacionamentos do objeto contact.</span><span class="sxs-lookup"><span data-stu-id="2d739-104">Retrieve the properties and relationships of a contact object.</span></span>

<span data-ttu-id="2d739-105">Há dois cenários em que um aplicativo pode obter um contato na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="2d739-105">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="2d739-106">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="2d739-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="2d739-107">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="2d739-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="2d739-108">Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="2d739-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="2d739-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d739-109">Permissions</span></span>
<span data-ttu-id="2d739-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d739-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d739-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d739-112">Permission type</span></span>      | <span data-ttu-id="2d739-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d739-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d739-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d739-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2d739-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d739-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2d739-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d739-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d739-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d739-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2d739-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d739-118">Application</span></span> | <span data-ttu-id="2d739-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d739-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d739-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d739-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="2d739-121">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="2d739-121">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="2d739-122">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="2d739-122">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="2d739-p103">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="2d739-p103">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d739-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2d739-125">Optional query parameters</span></span>
|<span data-ttu-id="2d739-126">Nome</span><span class="sxs-lookup"><span data-stu-id="2d739-126">Name</span></span>|<span data-ttu-id="2d739-127">Valor</span><span class="sxs-lookup"><span data-stu-id="2d739-127">Value</span></span>|<span data-ttu-id="2d739-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d739-128">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="2d739-129">$expand</span><span class="sxs-lookup"><span data-stu-id="2d739-129">$expand</span></span>|<span data-ttu-id="2d739-130">string</span><span class="sxs-lookup"><span data-stu-id="2d739-130">string</span></span>|<span data-ttu-id="2d739-p104">Lista separada por vírgulas de relações para expandir e incluir na resposta. Consulte a tabela de relacionamentos do objeto [contact](../resources/contact.md) para conhecer os nomes compatíveis.</span><span class="sxs-lookup"><span data-stu-id="2d739-p104">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="2d739-133">$select</span><span class="sxs-lookup"><span data-stu-id="2d739-133">$select</span></span>|<span data-ttu-id="2d739-134">string</span><span class="sxs-lookup"><span data-stu-id="2d739-134">string</span></span>|<span data-ttu-id="2d739-135">Lista separada por vírgulas de propriedades para incluir na resposta.</span><span class="sxs-lookup"><span data-stu-id="2d739-135">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2d739-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d739-136">Request headers</span></span>
| <span data-ttu-id="2d739-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d739-137">Header</span></span>       | <span data-ttu-id="2d739-138">Valor</span><span class="sxs-lookup"><span data-stu-id="2d739-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d739-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d739-139">Authorization</span></span>  | <span data-ttu-id="2d739-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d739-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d739-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d739-142">Request body</span></span>
<span data-ttu-id="2d739-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2d739-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d739-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d739-144">Response</span></span>

<span data-ttu-id="2d739-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d739-145">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d739-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d739-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d739-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d739-147">Request</span></span>
<span data-ttu-id="2d739-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d739-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2d739-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d739-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d739-150">C#</span><span class="sxs-lookup"><span data-stu-id="2d739-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d739-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="2d739-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d739-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2d739-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2d739-153">Java</span><span class="sxs-lookup"><span data-stu-id="2d739-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2d739-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d739-154">Response</span></span>
<span data-ttu-id="2d739-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d739-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
