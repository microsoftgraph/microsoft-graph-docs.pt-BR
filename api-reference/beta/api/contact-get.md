---
title: Obter contato
description: Recupere as propriedades e as relações do objeto de contato.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: accc9f8f8b089a5c4dc8a46bd3129806a9795bd8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472535"
---
# <a name="get-contact"></a><span data-ttu-id="25aa1-103">Obter contato</span><span class="sxs-lookup"><span data-stu-id="25aa1-103">Get contact</span></span>

<span data-ttu-id="25aa1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25aa1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25aa1-105">Recupere as propriedades e as relações do objeto de contato.</span><span class="sxs-lookup"><span data-stu-id="25aa1-105">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="25aa1-106">Há dois cenários em que um aplicativo pode obter um contato na pasta de contato de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="25aa1-106">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="25aa1-107">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="25aa1-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="25aa1-108">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="25aa1-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="25aa1-109">Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="25aa1-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="25aa1-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="25aa1-110">Permissions</span></span>
<span data-ttu-id="25aa1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25aa1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25aa1-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25aa1-113">Permission type</span></span>      | <span data-ttu-id="25aa1-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25aa1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25aa1-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25aa1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="25aa1-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25aa1-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="25aa1-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25aa1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25aa1-118">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25aa1-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="25aa1-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25aa1-119">Application</span></span> | <span data-ttu-id="25aa1-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25aa1-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="25aa1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25aa1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="25aa1-122">Um [contato](../resources/contact.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="25aa1-122">A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="25aa1-123">Um [contato](../resources/contact.md) de um [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="25aa1-123">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="25aa1-124">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="25aa1-124">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="25aa1-125">O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="25aa1-125">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="25aa1-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25aa1-126">Optional query parameters</span></span>
|<span data-ttu-id="25aa1-127">Nome</span><span class="sxs-lookup"><span data-stu-id="25aa1-127">Name</span></span>|<span data-ttu-id="25aa1-128">Valor</span><span class="sxs-lookup"><span data-stu-id="25aa1-128">Value</span></span>|<span data-ttu-id="25aa1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="25aa1-129">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="25aa1-130">$expand</span><span class="sxs-lookup"><span data-stu-id="25aa1-130">$expand</span></span>|<span data-ttu-id="25aa1-131">string</span><span class="sxs-lookup"><span data-stu-id="25aa1-131">string</span></span>|<span data-ttu-id="25aa1-132">Lista separada por vírgulas de relações para expandir e incluir na resposta.</span><span class="sxs-lookup"><span data-stu-id="25aa1-132">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="25aa1-133">Consulte relationships table of [contact](../resources/contact.md) object for supported names.</span><span class="sxs-lookup"><span data-stu-id="25aa1-133">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="25aa1-134">$select</span><span class="sxs-lookup"><span data-stu-id="25aa1-134">$select</span></span>|<span data-ttu-id="25aa1-135">string</span><span class="sxs-lookup"><span data-stu-id="25aa1-135">string</span></span>|<span data-ttu-id="25aa1-136">Lista separada por vírgulas de propriedades para incluir na resposta.</span><span class="sxs-lookup"><span data-stu-id="25aa1-136">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="25aa1-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25aa1-137">Request headers</span></span>
| <span data-ttu-id="25aa1-138">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25aa1-138">Header</span></span>       | <span data-ttu-id="25aa1-139">Valor</span><span class="sxs-lookup"><span data-stu-id="25aa1-139">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25aa1-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="25aa1-140">Authorization</span></span>  | <span data-ttu-id="25aa1-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25aa1-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25aa1-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25aa1-143">Request body</span></span>
<span data-ttu-id="25aa1-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25aa1-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25aa1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="25aa1-145">Response</span></span>

<span data-ttu-id="25aa1-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25aa1-146">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25aa1-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25aa1-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25aa1-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25aa1-148">Request</span></span>
<span data-ttu-id="25aa1-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25aa1-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="25aa1-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="25aa1-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
# <a name="c"></a>[<span data-ttu-id="25aa1-151">C#</span><span class="sxs-lookup"><span data-stu-id="25aa1-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25aa1-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25aa1-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25aa1-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25aa1-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25aa1-154">Java</span><span class="sxs-lookup"><span data-stu-id="25aa1-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="25aa1-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="25aa1-155">Response</span></span>
<span data-ttu-id="25aa1-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25aa1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com",
      "type": "unknown"
    },
    {
      "name": "Garth",
      "address": "garth@contoso.onmicrosoft.com",
      "type": "personal"
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
  "assistantName": null,
  "manager": null,
  "phones": [{
    "type": "business",
    "number": "+1 918 555 0101"
  }],
  "postalAddresses": [{
    "type": "business",
    "postOfficeBox": "P.O. Box 100",
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "countryOrRegion": "USA",
    "postalCode": "98121"
  }],
  "spouseName": null,
  "personalNotes": null,
  "children": [], 
  "gender": null,
  "websites": [{
      "type": "work",
      "address": "https://www.contoso.com",
      "name": "Contoso"
  }],
  "weddingAnniversary": null
}
```

## <a name="see-also"></a><span data-ttu-id="25aa1-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="25aa1-159">See also</span></span>

- [<span data-ttu-id="25aa1-160">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="25aa1-160">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="25aa1-161">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="25aa1-161">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


