---
title: Obter contato
description: Recupere as propriedades e relacionamentos de objeto de contato.
ms.openlocfilehash: 41784971e4e74fe34c4d0f55b8b0139ce3356e79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037808"
---
# <a name="get-contact"></a><span data-ttu-id="78e6d-103">Obter contato</span><span class="sxs-lookup"><span data-stu-id="78e6d-103">Get contact</span></span>

> <span data-ttu-id="78e6d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="78e6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78e6d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="78e6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78e6d-106">Recupere as propriedades e relacionamentos de objeto de contato.</span><span class="sxs-lookup"><span data-stu-id="78e6d-106">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="78e6d-107">Há dois cenários em que um aplicativo pode receber um contato na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="78e6d-107">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="78e6d-108">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="78e6d-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="78e6d-109">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de contato com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="78e6d-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="78e6d-110">Consulte os [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="78e6d-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="78e6d-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="78e6d-111">Permissions</span></span>
<span data-ttu-id="78e6d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78e6d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e6d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78e6d-114">Permission type</span></span>      | <span data-ttu-id="78e6d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78e6d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78e6d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78e6d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="78e6d-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78e6d-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="78e6d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78e6d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78e6d-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78e6d-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="78e6d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78e6d-120">Application</span></span> | <span data-ttu-id="78e6d-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78e6d-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="78e6d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78e6d-122">HTTP request</span></span>
<span data-ttu-id="78e6d-123"><!-- { "blockType": "ignored" } -->Um [contato](../resources/contact.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="78e6d-123"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="78e6d-124">Um [contato](../resources/contact.md) de um nível superior [contactFolder](../resources/contactfolder.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="78e6d-124">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="78e6d-125">Um [contato](../resources/contact.md) contidos em uma pasta filho de um [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="78e6d-125">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="78e6d-126">O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado no filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="78e6d-126">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78e6d-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78e6d-127">Optional query parameters</span></span>
|<span data-ttu-id="78e6d-128">Nome</span><span class="sxs-lookup"><span data-stu-id="78e6d-128">Name</span></span>|<span data-ttu-id="78e6d-129">Valor</span><span class="sxs-lookup"><span data-stu-id="78e6d-129">Value</span></span>|<span data-ttu-id="78e6d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="78e6d-130">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="78e6d-131">$expand</span><span class="sxs-lookup"><span data-stu-id="78e6d-131">$expand</span></span>|<span data-ttu-id="78e6d-132">string</span><span class="sxs-lookup"><span data-stu-id="78e6d-132">string</span></span>|<span data-ttu-id="78e6d-133">Lista separada por vírgulas de relações para expandir e incluir na resposta.</span><span class="sxs-lookup"><span data-stu-id="78e6d-133">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="78e6d-134">Consulte a tabela de relações do objeto de [contato](../resources/contact.md) para nomes com suporte.</span><span class="sxs-lookup"><span data-stu-id="78e6d-134">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="78e6d-135">$select</span><span class="sxs-lookup"><span data-stu-id="78e6d-135">$select</span></span>|<span data-ttu-id="78e6d-136">string</span><span class="sxs-lookup"><span data-stu-id="78e6d-136">string</span></span>|<span data-ttu-id="78e6d-137">Lista separada por vírgulas de propriedades para incluir na resposta.</span><span class="sxs-lookup"><span data-stu-id="78e6d-137">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="78e6d-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78e6d-138">Request headers</span></span>
| <span data-ttu-id="78e6d-139">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78e6d-139">Header</span></span>       | <span data-ttu-id="78e6d-140">Valor</span><span class="sxs-lookup"><span data-stu-id="78e6d-140">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="78e6d-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="78e6d-141">Authorization</span></span>  | <span data-ttu-id="78e6d-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78e6d-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="78e6d-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78e6d-144">Request body</span></span>
<span data-ttu-id="78e6d-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78e6d-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78e6d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e6d-146">Response</span></span>

<span data-ttu-id="78e6d-147">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78e6d-147">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78e6d-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78e6d-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78e6d-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78e6d-149">Request</span></span>
<span data-ttu-id="78e6d-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78e6d-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
##### <a name="response"></a><span data-ttu-id="78e6d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e6d-151">Response</span></span>
<span data-ttu-id="78e6d-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78e6d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="78e6d-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="78e6d-155">See also</span></span>

- [<span data-ttu-id="78e6d-156">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="78e6d-156">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="78e6d-157">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="78e6d-157">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->