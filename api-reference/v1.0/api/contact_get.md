# <a name="get-contact"></a><span data-ttu-id="9a23d-101">Obter contato</span><span class="sxs-lookup"><span data-stu-id="9a23d-101">Get contact</span></span>

<span data-ttu-id="9a23d-102">Recupere as propriedades e os relacionamentos do objeto contact.</span><span class="sxs-lookup"><span data-stu-id="9a23d-102">Retrieve the properties and relationships of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a23d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a23d-103">Permissions</span></span>
<span data-ttu-id="9a23d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a23d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a23d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a23d-106">Permission type</span></span>      | <span data-ttu-id="9a23d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a23d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a23d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a23d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9a23d-109">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a23d-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9a23d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a23d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a23d-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a23d-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9a23d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a23d-112">Application</span></span> | <span data-ttu-id="9a23d-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a23d-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a23d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a23d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9a23d-115">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="9a23d-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="9a23d-116">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="9a23d-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="9a23d-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="9a23d-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a23d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a23d-119">Optional query parameters</span></span>
|<span data-ttu-id="9a23d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9a23d-120">Name</span></span>|<span data-ttu-id="9a23d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9a23d-121">Value</span></span>|<span data-ttu-id="9a23d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a23d-122">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="9a23d-123">$expand</span><span class="sxs-lookup"><span data-stu-id="9a23d-123">$expand</span></span>|<span data-ttu-id="9a23d-124">string</span><span class="sxs-lookup"><span data-stu-id="9a23d-124">string</span></span>|<span data-ttu-id="9a23d-p103">Lista separada por vírgulas de relações para expandir e incluir na resposta. Consulte a tabela de relacionamentos do objeto [contact](../resources/contact.md) para conhecer os nomes compatíveis.</span><span class="sxs-lookup"><span data-stu-id="9a23d-p103">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="9a23d-127">$select</span><span class="sxs-lookup"><span data-stu-id="9a23d-127">$select</span></span>|<span data-ttu-id="9a23d-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a23d-128">string</span></span>|<span data-ttu-id="9a23d-129">Lista separada por vírgulas de propriedades para incluir na resposta.</span><span class="sxs-lookup"><span data-stu-id="9a23d-129">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9a23d-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a23d-130">Request headers</span></span>
| <span data-ttu-id="9a23d-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a23d-131">Header</span></span>       | <span data-ttu-id="9a23d-132">Valor</span><span class="sxs-lookup"><span data-stu-id="9a23d-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a23d-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a23d-133">Authorization</span></span>  | <span data-ttu-id="9a23d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a23d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a23d-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a23d-136">Request body</span></span>
<span data-ttu-id="9a23d-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a23d-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a23d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a23d-138">Response</span></span>

<span data-ttu-id="9a23d-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a23d-139">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a23d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a23d-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a23d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a23d-141">Request</span></span>
<span data-ttu-id="9a23d-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a23d-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="9a23d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a23d-143">Response</span></span>
<span data-ttu-id="9a23d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a23d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "http://www.contoso.com",
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
