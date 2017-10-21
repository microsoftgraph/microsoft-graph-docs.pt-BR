# <a name="get-contact"></a><span data-ttu-id="45faf-101">Obter contato</span><span class="sxs-lookup"><span data-stu-id="45faf-101">Get contact</span></span>

<span data-ttu-id="45faf-102">Recupere as propriedades e os relacionamentos do objeto contact.</span><span class="sxs-lookup"><span data-stu-id="45faf-102">Retrieve the properties and relationships of a contact object.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="45faf-103">Obter contatos na pasta de contatos de outro usuário</span><span class="sxs-lookup"><span data-stu-id="45faf-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="45faf-104">Se você tiver permissões de aplicativo ou se você tiver as [permissões](#permissions) delegadas apropriadas de um usuário, será possível obter os contatos da pasta de contatos de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="45faf-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="45faf-105">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="45faf-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="45faf-106">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="45faf-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="45faf-107">Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de contatos com Diogo.</span><span class="sxs-lookup"><span data-stu-id="45faf-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="45faf-108">Você pode obter um contato nessa pasta compartilhada especificando a ID de usuário de Henrique (ou o nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="45faf-108">You can get a contact in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts/{id}
```

<span data-ttu-id="45faf-109">Esse recurso se aplica a todas as operações de contatos GET com suporte para usuários individuais, conforme listado na seção [solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="45faf-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="45faf-110">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="45faf-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="45faf-111">Se Henrique não tiver compartilhado sua pasta de contatos com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="45faf-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="45faf-112">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para obter um contato nas próprias pastas de contatos do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="45faf-112">In such cases, specifying a user ID or user principal name only works for getting a contact in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}
```

<span data-ttu-id="45faf-113">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="45faf-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="45faf-114">Pastas de contatos compartilhadas</span><span class="sxs-lookup"><span data-stu-id="45faf-114">Shared contact folders</span></span>
- <span data-ttu-id="45faf-115">Calendários compartilhados</span><span class="sxs-lookup"><span data-stu-id="45faf-115">Shared calendars</span></span>
- <span data-ttu-id="45faf-116">Contatos e eventos em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="45faf-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="45faf-117">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="45faf-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="45faf-118">Esse recurso não está disponível em outras operações para contatos, eventos e suas pastas.</span><span class="sxs-lookup"><span data-stu-id="45faf-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="45faf-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="45faf-119">Permissions</span></span>
<span data-ttu-id="45faf-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="45faf-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="45faf-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45faf-122">Permission type</span></span>      | <span data-ttu-id="45faf-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45faf-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45faf-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45faf-124">Delegated (work or school account)</span></span> | <span data-ttu-id="45faf-125">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45faf-125">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="45faf-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45faf-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45faf-127">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45faf-127">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="45faf-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45faf-128">Application</span></span> | <span data-ttu-id="45faf-129">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45faf-129">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="45faf-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45faf-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="45faf-131">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="45faf-131">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="45faf-132">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="45faf-132">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="45faf-p106">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="45faf-p106">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="45faf-135">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45faf-135">Optional query parameters</span></span>
|<span data-ttu-id="45faf-136">Nome</span><span class="sxs-lookup"><span data-stu-id="45faf-136">Name</span></span>|<span data-ttu-id="45faf-137">Valor</span><span class="sxs-lookup"><span data-stu-id="45faf-137">Value</span></span>|<span data-ttu-id="45faf-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="45faf-138">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="45faf-139">$expand</span><span class="sxs-lookup"><span data-stu-id="45faf-139">$expand</span></span>|<span data-ttu-id="45faf-140">string</span><span class="sxs-lookup"><span data-stu-id="45faf-140">string</span></span>|<span data-ttu-id="45faf-p107">Lista separada por vírgulas de relações para expandir e incluir na resposta. Consulte a tabela de relacionamentos do objeto [contact](../resources/contact.md) para conhecer os nomes compatíveis.</span><span class="sxs-lookup"><span data-stu-id="45faf-p107">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="45faf-143">$select</span><span class="sxs-lookup"><span data-stu-id="45faf-143">$select</span></span>|<span data-ttu-id="45faf-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45faf-144">string</span></span>|<span data-ttu-id="45faf-145">Lista separada por vírgulas de propriedades para incluir na resposta.</span><span class="sxs-lookup"><span data-stu-id="45faf-145">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="45faf-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45faf-146">Request headers</span></span>
| <span data-ttu-id="45faf-147">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45faf-147">Header</span></span>       | <span data-ttu-id="45faf-148">Valor</span><span class="sxs-lookup"><span data-stu-id="45faf-148">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="45faf-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="45faf-149">Authorization</span></span>  | <span data-ttu-id="45faf-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45faf-p108">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="45faf-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45faf-152">Request body</span></span>
<span data-ttu-id="45faf-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45faf-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45faf-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="45faf-154">Response</span></span>

<span data-ttu-id="45faf-155">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45faf-155">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45faf-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45faf-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45faf-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45faf-157">Request</span></span>
<span data-ttu-id="45faf-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45faf-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="45faf-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="45faf-159">Response</span></span>
<span data-ttu-id="45faf-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45faf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
