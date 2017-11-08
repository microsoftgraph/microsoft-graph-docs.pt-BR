# <a name="list-messages"></a><span data-ttu-id="3b5eb-101">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="3b5eb-101">List messages</span></span>

<span data-ttu-id="3b5eb-102">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="3b5eb-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="3b5eb-103">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-103">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="3b5eb-104">Receber mensagens na pasta de mensagens de outro usuário</span><span class="sxs-lookup"><span data-stu-id="3b5eb-104">Get messages in another user's message folder</span></span>

<span data-ttu-id="3b5eb-105">Se você tem permissões de aplicativo ou as [permissões](#permissions) delegadas apropriadas de um usuário, é possível receber mensagens da pasta de mensagens de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="3b5eb-106">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="3b5eb-107">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="3b5eb-108">Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de mensagens com Diogo.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-108">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="3b5eb-109">Você pode receber mensagens nessa pasta compartilhada especificando a ID de usuário do Henrique (ou o nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-109">You can get the contacts in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages
```

<span data-ttu-id="3b5eb-110">Esse recurso se aplica a todas as operações de mensagens GET com suporte a usuários individuais, como mostra a seção [Solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-110">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="3b5eb-111">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="3b5eb-112">Se Henrique não tiver compartilhado a pasta de mensagens dele com Diogo nem delegado a caixa de correio dele a Diogo, a especificação da ID de usuário do Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-112">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="3b5eb-113">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para receber mensagens nas próprias pastas de mensagens do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="3b5eb-113">In such cases, specifying a user ID or user principal name only works for getting contacts in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
```

<span data-ttu-id="3b5eb-114">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="3b5eb-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="3b5eb-115">Pastas de contatos, calendários e pastas de mensagens compartilhados</span><span class="sxs-lookup"><span data-stu-id="3b5eb-115">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="3b5eb-116">Contatos, eventos e mensagens em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="3b5eb-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="3b5eb-117">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="3b5eb-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="3b5eb-118">Esse recurso não está disponível em outras operações para contatos, eventos, mensagens e respectivas pastas.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="3b5eb-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b5eb-119">Permissions</span></span>
<span data-ttu-id="3b5eb-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3b5eb-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b5eb-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b5eb-122">Permission type</span></span>      | <span data-ttu-id="3b5eb-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b5eb-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b5eb-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b5eb-124">Delegated (work or school account)</span></span> | <span data-ttu-id="3b5eb-125">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b5eb-125">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3b5eb-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b5eb-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b5eb-127">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b5eb-127">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3b5eb-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b5eb-128">Application</span></span> | <span data-ttu-id="3b5eb-129">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b5eb-129">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b5eb-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b5eb-130">HTTP request</span></span>

<span data-ttu-id="3b5eb-131">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="3b5eb-131">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="3b5eb-132">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="3b5eb-132">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b5eb-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3b5eb-133">Optional query parameters</span></span>
<span data-ttu-id="3b5eb-134">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-134">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3b5eb-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b5eb-135">Request headers</span></span>
| <span data-ttu-id="3b5eb-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b5eb-136">Header</span></span>       | <span data-ttu-id="3b5eb-137">Valor</span><span class="sxs-lookup"><span data-stu-id="3b5eb-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b5eb-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b5eb-138">Authorization</span></span>  | <span data-ttu-id="3b5eb-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b5eb-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b5eb-141">Request body</span></span>
<span data-ttu-id="3b5eb-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b5eb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b5eb-143">Response</span></span>

<span data-ttu-id="3b5eb-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-144">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="3b5eb-145">O tamanho de página padrão para essa solicitação é dez mensagens.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-145">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="3b5eb-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b5eb-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b5eb-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b5eb-147">Request</span></span>
<span data-ttu-id="3b5eb-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="3b5eb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b5eb-149">Response</span></span>
<span data-ttu-id="3b5eb-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b5eb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
