# <a name="get-contactfolder"></a><span data-ttu-id="24548-101">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="24548-101">Get contactFolder</span></span>

<span data-ttu-id="24548-102">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="24548-102">Get a contact folder by using the contact folder ID.</span></span>


### <a name="get-another-users-contact-folder"></a><span data-ttu-id="24548-103">Obter a pasta de contatos de outro usuário</span><span class="sxs-lookup"><span data-stu-id="24548-103">Get another user's contact folder</span></span>

<span data-ttu-id="24548-104">Se você tiver permissões de aplicativo ou se tiver as [permissões](#permissions) delegadas apropriadas de um usuário, será possível obter a pasta de contatos de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="24548-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to a get contact folder of another user's.</span></span> <span data-ttu-id="24548-105">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="24548-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="24548-106">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="24548-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="24548-107">Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de contatos com Diogo.</span><span class="sxs-lookup"><span data-stu-id="24548-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="24548-108">Você pode obter essa pasta compartilhada especificando a ID de usuário de Henrique (ou nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="24548-108">You can get that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contactFolders/{id}
```

<span data-ttu-id="24548-109">Esse recurso se aplica a todas as operações de pastas de contatos GET para usuários individuais, conforme descrito na seção [Solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="24548-109">This capability applies to all GET contact folder operations for an individual user, as described in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="24548-110">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="24548-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="24548-111">Se Henrique não tiver compartilhado sua pasta de contatos com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="24548-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="24548-112">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para obter a pasta de contatos do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="24548-112">In such cases, specifying a user ID or user principal name only works for getting a contact folder of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
```

<span data-ttu-id="24548-113">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="24548-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="24548-114">Pastas de contatos, calendários e pastas de mensagens compartilhados</span><span class="sxs-lookup"><span data-stu-id="24548-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="24548-115">Contatos, eventos e mensagens em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="24548-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="24548-116">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="24548-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="24548-117">Esse recurso não está disponível em outras operações para contatos, eventos, mensagens e respectivas pastas.</span><span class="sxs-lookup"><span data-stu-id="24548-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="24548-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="24548-118">Permissions</span></span>
<span data-ttu-id="24548-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24548-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24548-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24548-121">Permission type</span></span>      | <span data-ttu-id="24548-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24548-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24548-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24548-123">Delegated (work or school account)</span></span> | <span data-ttu-id="24548-124">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24548-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="24548-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24548-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24548-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24548-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="24548-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24548-127">Application</span></span> | <span data-ttu-id="24548-128">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24548-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="24548-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24548-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="24548-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24548-130">Optional query parameters</span></span>
<span data-ttu-id="24548-131">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24548-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="24548-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24548-132">Request headers</span></span>
| <span data-ttu-id="24548-133">Nome</span><span class="sxs-lookup"><span data-stu-id="24548-133">Name</span></span>       | <span data-ttu-id="24548-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="24548-134">Type</span></span> | <span data-ttu-id="24548-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="24548-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="24548-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="24548-136">Authorization</span></span>  | <span data-ttu-id="24548-137">string</span><span class="sxs-lookup"><span data-stu-id="24548-137">string</span></span>  | <span data-ttu-id="24548-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24548-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24548-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24548-140">Request body</span></span>
<span data-ttu-id="24548-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24548-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24548-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="24548-142">Response</span></span>

<span data-ttu-id="24548-143">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24548-143">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24548-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24548-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24548-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24548-145">Request</span></span>
<span data-ttu-id="24548-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24548-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="24548-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="24548-147">Response</span></span>
<span data-ttu-id="24548-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24548-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
