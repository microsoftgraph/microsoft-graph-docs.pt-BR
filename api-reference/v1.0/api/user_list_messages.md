# <a name="list-messages"></a><span data-ttu-id="dd38e-101">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="dd38e-101">List messages</span></span>

<span data-ttu-id="dd38e-102">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="dd38e-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="dd38e-103">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="dd38e-103">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="dd38e-104">Receber mensagens na pasta de mensagens de outro usuário</span><span class="sxs-lookup"><span data-stu-id="dd38e-104">Get messages in another user's message folder</span></span>

<span data-ttu-id="dd38e-105">Se você tem permissões de aplicativo ou as [permissões](#permissions) delegadas apropriadas de um usuário, é possível receber mensagens da pasta de mensagens de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="dd38e-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get messages from another user's message folder.</span></span> <span data-ttu-id="dd38e-106">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="dd38e-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="dd38e-107">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="dd38e-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="dd38e-108">Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de mensagens com Diogo.</span><span class="sxs-lookup"><span data-stu-id="dd38e-108">Suppose another user, Garth, has shared a message folder with John.</span></span> <span data-ttu-id="dd38e-109">Você pode receber mensagens nessa pasta compartilhada especificando a ID de usuário do Henrique (ou o nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="dd38e-109">You can get the messages in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages
```

<span data-ttu-id="dd38e-110">Esse recurso se aplica a todas as operações de mensagens GET com suporte a usuários individuais, como mostra a seção [Solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="dd38e-110">This capability applies to all the supported GET messages operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="dd38e-111">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="dd38e-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="dd38e-112">Se Henrique não tiver compartilhado a pasta de mensagens dele com Diogo nem delegado a caixa de correio dele a Diogo, a especificação da ID de usuário do Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="dd38e-112">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="dd38e-113">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para receber mensagens nas próprias pastas de mensagens do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="dd38e-113">In such cases, specifying a user ID or user principal name only works for getting messages in the signed-in user’s own message folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
```

<span data-ttu-id="dd38e-114">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="dd38e-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="dd38e-115">Pastas de contatos, calendários e pastas de mensagens compartilhados</span><span class="sxs-lookup"><span data-stu-id="dd38e-115">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="dd38e-116">Contatos, eventos e mensagens em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="dd38e-116">Contacts, events, and messages in shared folders</span></span>
- <span data-ttu-id="dd38e-117">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="dd38e-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="dd38e-118">Esse recurso não está disponível em outras operações para contatos, eventos, mensagens e respectivas pastas.</span><span class="sxs-lookup"><span data-stu-id="dd38e-118">This capability is not available in other operations for contacts, events, messages, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="dd38e-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd38e-119">Permissions</span></span>
<span data-ttu-id="dd38e-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd38e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dd38e-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd38e-122">Permission type</span></span>      | <span data-ttu-id="dd38e-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd38e-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd38e-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd38e-124">Delegated (work or school account)</span></span> | <span data-ttu-id="dd38e-125">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd38e-125">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd38e-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd38e-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd38e-127">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd38e-127">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd38e-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd38e-128">Application</span></span> | <span data-ttu-id="dd38e-129">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd38e-129">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd38e-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd38e-130">HTTP request</span></span>

<span data-ttu-id="dd38e-131">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="dd38e-131">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="dd38e-132">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="dd38e-132">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd38e-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dd38e-133">Optional query parameters</span></span>
<span data-ttu-id="dd38e-134">Este método dá suporte a [Parâmetros de consulta OData]((http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters)) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dd38e-134">This method supports the [OData Query Parameters]((http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dd38e-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd38e-135">Request headers</span></span>
| <span data-ttu-id="dd38e-136">Nome</span><span class="sxs-lookup"><span data-stu-id="dd38e-136">Name</span></span>       | <span data-ttu-id="dd38e-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd38e-137">Type</span></span> | <span data-ttu-id="dd38e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd38e-138">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dd38e-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd38e-139">Authorization</span></span>  | <span data-ttu-id="dd38e-140">string</span><span class="sxs-lookup"><span data-stu-id="dd38e-140">string</span></span>  | <span data-ttu-id="dd38e-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd38e-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd38e-143">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="dd38e-143">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="dd38e-144">string</span><span class="sxs-lookup"><span data-stu-id="dd38e-144">string</span></span> | <span data-ttu-id="dd38e-145">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="dd38e-145">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="dd38e-146">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="dd38e-146">Values can be "text" or "html".</span></span> <span data-ttu-id="dd38e-147">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="dd38e-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="dd38e-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dd38e-148">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="dd38e-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd38e-149">Request body</span></span>
<span data-ttu-id="dd38e-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd38e-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd38e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd38e-151">Response</span></span>

<span data-ttu-id="dd38e-152">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd38e-152">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="dd38e-153">O tamanho de página padrão para essa solicitação é dez mensagens.</span><span class="sxs-lookup"><span data-stu-id="dd38e-153">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="dd38e-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd38e-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd38e-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd38e-155">Request</span></span>
<span data-ttu-id="dd38e-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd38e-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="dd38e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd38e-157">Response</span></span>
<span data-ttu-id="dd38e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd38e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
