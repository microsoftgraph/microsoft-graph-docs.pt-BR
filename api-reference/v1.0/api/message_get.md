# <a name="get-message"></a><span data-ttu-id="6a209-101">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="6a209-101">Get message</span></span>

<span data-ttu-id="6a209-102">Recupere as propriedades e os relacionamentos de um objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="6a209-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="6a209-103">Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="6a209-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="6a209-104">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="6a209-104">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="6a209-105">Receber mensagens na pasta de mensagens de outro usuário</span><span class="sxs-lookup"><span data-stu-id="6a209-105">Get messages in another user's message folder</span></span>

<span data-ttu-id="6a209-106">Se você tem permissões de aplicativo ou as [permissões](#permissions) delegadas apropriadas de um usuário, é possível receber mensagens da pasta de mensagens de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="6a209-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="6a209-107">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="6a209-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="6a209-108">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="6a209-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="6a209-109">Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de mensagens com Diogo.</span><span class="sxs-lookup"><span data-stu-id="6a209-109">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="6a209-110">Você pode receber mensagem nessa pasta compartilhada especificando a ID de usuário do Henrique (ou o nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="6a209-110">You can get a contact in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages/{id}
```

<span data-ttu-id="6a209-111">Esse recurso se aplica a todas as operações de mensagens GET com suporte a usuários individuais, como mostra a seção [Solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="6a209-111">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="6a209-112">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="6a209-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="6a209-113">Se Henrique não tiver compartilhado a pasta de mensagens dele com Diogo nem delegado a caixa de correio dele a Diogo, a especificação da ID de usuário do Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="6a209-113">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="6a209-114">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para receber uma mensagem nas próprias pastas de mensagens do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="6a209-114">In such cases, specifying a user ID or user principal name only works for getting a contact in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
```

<span data-ttu-id="6a209-115">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="6a209-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="6a209-116">Pastas de contatos, calendários e pastas de mensagens compartilhados</span><span class="sxs-lookup"><span data-stu-id="6a209-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="6a209-117">Contatos, eventos e mensagens em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="6a209-117">Contacts and events in shared folders</span></span>
- <span data-ttu-id="6a209-118">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="6a209-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="6a209-119">Esse recurso não está disponível em outras operações para contatos, eventos, mensagens e respectivas pastas.</span><span class="sxs-lookup"><span data-stu-id="6a209-119">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="6a209-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a209-120">Permissions</span></span>
<span data-ttu-id="6a209-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a209-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6a209-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a209-123">Permission type</span></span>      | <span data-ttu-id="6a209-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a209-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a209-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a209-125">Delegated (work or school account)</span></span> | <span data-ttu-id="6a209-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a209-126">Mail.Read</span></span>    |
|<span data-ttu-id="6a209-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a209-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a209-128">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a209-128">Mail.Read</span></span>    |
|<span data-ttu-id="6a209-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a209-129">Application</span></span> | <span data-ttu-id="6a209-130">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a209-130">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a209-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a209-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a209-132">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a209-132">Optional query parameters</span></span>
<span data-ttu-id="6a209-133">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a209-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6a209-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a209-134">Request headers</span></span>
| <span data-ttu-id="6a209-135">Nome</span><span class="sxs-lookup"><span data-stu-id="6a209-135">Name</span></span>       | <span data-ttu-id="6a209-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a209-136">Type</span></span> | <span data-ttu-id="6a209-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a209-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a209-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a209-138">Authorization</span></span>  | <span data-ttu-id="6a209-139">string</span><span class="sxs-lookup"><span data-stu-id="6a209-139">string</span></span>  | <span data-ttu-id="6a209-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a209-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a209-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a209-142">Request body</span></span>
<span data-ttu-id="6a209-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a209-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a209-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a209-144">Response</span></span>

<span data-ttu-id="6a209-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a209-145">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a209-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a209-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a209-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a209-147">Request</span></span>
<span data-ttu-id="6a209-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a209-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="6a209-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a209-149">Response</span></span>
<span data-ttu-id="6a209-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a209-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="6a209-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="6a209-153">See also</span></span>

- [<span data-ttu-id="6a209-154">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="6a209-154">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="6a209-155">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="6a209-155">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
