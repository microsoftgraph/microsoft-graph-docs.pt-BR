# <a name="get-message"></a><span data-ttu-id="45023-101">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="45023-101">Get message</span></span>

<span data-ttu-id="45023-102">Recupere as propriedades e os relacionamentos de um objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="45023-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="45023-103">Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="45023-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="45023-104">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="45023-104">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="45023-105">Receber mensagens na pasta de mensagens de outro usuário</span><span class="sxs-lookup"><span data-stu-id="45023-105">Get messages in another user's message folder</span></span>

<span data-ttu-id="45023-106">Se você tem permissões de aplicativo ou as [permissões](#permissions) delegadas apropriadas de um usuário, é possível receber mensagens da pasta de mensagens de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="45023-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get messages from another user's message folder.</span></span> <span data-ttu-id="45023-107">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="45023-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="45023-108">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="45023-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="45023-109">Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de mensagens com Diogo.</span><span class="sxs-lookup"><span data-stu-id="45023-109">Suppose another user, Garth, has shared a message folder with John.</span></span> <span data-ttu-id="45023-110">Você pode receber mensagem nessa pasta compartilhada especificando a ID de usuário do Henrique (ou o nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="45023-110">You can get a message in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages/{id}
```

<span data-ttu-id="45023-111">Esse recurso se aplica a todas as operações de mensagens GET com suporte a usuários individuais, como mostra a seção [Solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="45023-111">This capability applies to all the supported GET messages operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="45023-112">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="45023-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="45023-113">Se Henrique não tiver compartilhado a pasta de mensagens dele com Diogo nem delegado a caixa de correio dele a Diogo, a especificação da ID de usuário do Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="45023-113">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="45023-114">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para receber uma mensagem nas próprias pastas de mensagens do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="45023-114">In such cases, specifying a user ID or user principal name only works for getting a message in the signed-in user’s own message folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
```

<span data-ttu-id="45023-115">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="45023-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="45023-116">Pastas de contatos, calendários e pastas de mensagens compartilhados</span><span class="sxs-lookup"><span data-stu-id="45023-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="45023-117">Contatos, eventos e mensagens em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="45023-117">Contacts, events, and messages in shared folders</span></span>
- <span data-ttu-id="45023-118">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="45023-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="45023-119">Esse recurso não está disponível em outras operações para contatos, eventos, mensagens e respectivas pastas.</span><span class="sxs-lookup"><span data-stu-id="45023-119">This capability is not available in other operations for contacts, events, messages, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="45023-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="45023-120">Permissions</span></span>
<span data-ttu-id="45023-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="45023-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="45023-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45023-123">Permission type</span></span>      | <span data-ttu-id="45023-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45023-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45023-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45023-125">Delegated (work or school account)</span></span> | <span data-ttu-id="45023-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="45023-126">Mail.Read</span></span>    |
|<span data-ttu-id="45023-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45023-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45023-128">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="45023-128">Mail.Read</span></span>    |
|<span data-ttu-id="45023-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45023-129">Application</span></span> | <span data-ttu-id="45023-130">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="45023-130">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="45023-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45023-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="45023-132">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45023-132">Optional query parameters</span></span>
<span data-ttu-id="45023-133">Este método dá suporte a [Parâmetros de consulta OData]((http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters)) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45023-133">This method supports the [OData Query Parameters]((http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="45023-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45023-134">Request headers</span></span>
| <span data-ttu-id="45023-135">Nome</span><span class="sxs-lookup"><span data-stu-id="45023-135">Name</span></span>       | <span data-ttu-id="45023-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="45023-136">Type</span></span> | <span data-ttu-id="45023-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="45023-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="45023-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="45023-138">Authorization</span></span>  | <span data-ttu-id="45023-139">string</span><span class="sxs-lookup"><span data-stu-id="45023-139">string</span></span>  | <span data-ttu-id="45023-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45023-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45023-142">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="45023-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="45023-143">string</span><span class="sxs-lookup"><span data-stu-id="45023-143">string</span></span> | <span data-ttu-id="45023-144">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="45023-144">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="45023-145">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="45023-145">Values can be "text" or "html".</span></span> <span data-ttu-id="45023-146">Um cabeçalho `Preference-Applied` é retornado como confirmação quando este cabeçalho `Prefer` é especificado.</span><span class="sxs-lookup"><span data-stu-id="45023-146">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="45023-147">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="45023-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="45023-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="45023-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45023-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45023-149">Request body</span></span>
<span data-ttu-id="45023-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45023-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45023-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="45023-151">Response</span></span>

<span data-ttu-id="45023-152">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45023-152">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45023-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45023-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45023-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45023-154">Request</span></span>
<span data-ttu-id="45023-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45023-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="45023-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="45023-156">Response</span></span>
<span data-ttu-id="45023-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45023-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="45023-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="45023-160">See also</span></span>

- [<span data-ttu-id="45023-161">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="45023-161">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="45023-162">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="45023-162">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
