# <a name="list-contacts"></a><span data-ttu-id="2e610-101">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="2e610-101">List contacts</span></span>

<span data-ttu-id="2e610-102">Obter uma coleção de contatos da pasta Contatos padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2e610-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="2e610-103">Obter contatos na pasta de contatos de outro usuário</span><span class="sxs-lookup"><span data-stu-id="2e610-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="2e610-104">Se você tiver permissões de aplicativo ou se você tiver as [permissões](#permissions) delegadas apropriadas de um usuário, será possível obter os contatos da pasta de contatos de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="2e610-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="2e610-105">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="2e610-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="2e610-106">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="2e610-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="2e610-107">Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de contatos com Diogo.</span><span class="sxs-lookup"><span data-stu-id="2e610-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="2e610-108">Você pode obter os contatos nessa pasta compartilhada especificando a ID de usuário de Henrique (ou o nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="2e610-108">You can get the contacts in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts
```

<span data-ttu-id="2e610-109">Esse recurso se aplica a todas as operações de contatos GET com suporte para usuários individuais, conforme listado na seção [solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="2e610-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="2e610-110">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="2e610-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="2e610-111">Se Henrique não tiver compartilhado sua pasta de contatos com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="2e610-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="2e610-112">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para obter contatos nas próprias pastas de contatos do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="2e610-112">In such cases, specifying a user ID or user principal name only works for getting contacts in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
```

<span data-ttu-id="2e610-113">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="2e610-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="2e610-114">Pastas de contatos compartilhadas</span><span class="sxs-lookup"><span data-stu-id="2e610-114">Shared contact folders</span></span>
- <span data-ttu-id="2e610-115">Calendários compartilhados</span><span class="sxs-lookup"><span data-stu-id="2e610-115">Shared calendars</span></span>
- <span data-ttu-id="2e610-116">Contatos e eventos em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="2e610-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="2e610-117">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="2e610-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="2e610-118">Esse recurso não está disponível em outras operações para contatos, eventos e suas pastas.</span><span class="sxs-lookup"><span data-stu-id="2e610-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="2e610-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e610-119">Permissions</span></span>
<span data-ttu-id="2e610-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e610-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e610-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e610-122">Permission type</span></span>      | <span data-ttu-id="2e610-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e610-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e610-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e610-124">Delegated (work or school account)</span></span> | <span data-ttu-id="2e610-125">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e610-125">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2e610-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e610-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e610-127">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e610-127">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2e610-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e610-128">Application</span></span> | <span data-ttu-id="2e610-129">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e610-129">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e610-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e610-130">HTTP request</span></span>

<span data-ttu-id="2e610-131">Para obter todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="2e610-131">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="2e610-132">Para obter os contatos em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="2e610-132">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e610-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e610-133">Optional query parameters</span></span>
<span data-ttu-id="2e610-134">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e610-134">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2e610-135">Por exemplo, você pode usar o parâmetro de consulta `$filter` para filtrar os contatos com base no domínio dos endereços de email deles:</span><span class="sxs-lookup"><span data-stu-id="2e610-135">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="2e610-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e610-136">Request headers</span></span>
| <span data-ttu-id="2e610-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e610-137">Header</span></span>       | <span data-ttu-id="2e610-138">Valor</span><span class="sxs-lookup"><span data-stu-id="2e610-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e610-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e610-139">Authorization</span></span>  | <span data-ttu-id="2e610-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e610-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2e610-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e610-142">Content-Type</span></span>   | <span data-ttu-id="2e610-143">application/json</span><span class="sxs-lookup"><span data-stu-id="2e610-143">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e610-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e610-144">Request body</span></span>
<span data-ttu-id="2e610-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e610-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e610-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e610-146">Response</span></span>

<span data-ttu-id="2e610-147">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e610-147">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e610-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e610-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e610-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e610-149">Request</span></span>
<span data-ttu-id="2e610-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e610-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="2e610-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e610-151">Response</span></span>
<span data-ttu-id="2e610-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e610-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
