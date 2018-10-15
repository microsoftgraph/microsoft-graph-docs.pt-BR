# <a name="get-conversation-thread"></a><span data-ttu-id="b8eed-101">Obter thread de conversas</span><span class="sxs-lookup"><span data-stu-id="b8eed-101">Get conversation thread</span></span>
<span data-ttu-id="b8eed-102">Obter um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="b8eed-102">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8eed-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8eed-103">Permissions</span></span>
<span data-ttu-id="b8eed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8eed-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8eed-106">Permission type</span></span>      | <span data-ttu-id="b8eed-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8eed-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8eed-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8eed-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b8eed-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8eed-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8eed-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8eed-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8eed-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8eed-111">Not supported.</span></span>    |
|<span data-ttu-id="b8eed-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8eed-112">Application</span></span> | <span data-ttu-id="b8eed-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8eed-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8eed-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8eed-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8eed-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8eed-115">Optional query parameters</span></span>
<span data-ttu-id="b8eed-116">Este método dá suporte a [Parâmetros de consulta OData](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8eed-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8eed-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8eed-117">Request headers</span></span>
| <span data-ttu-id="b8eed-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8eed-118">Header</span></span>       | <span data-ttu-id="b8eed-119">Valor</span><span class="sxs-lookup"><span data-stu-id="b8eed-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8eed-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8eed-120">Authorization</span></span>  | <span data-ttu-id="b8eed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8eed-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8eed-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8eed-123">Request body</span></span>
<span data-ttu-id="b8eed-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8eed-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8eed-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8eed-125">Response</span></span>
<span data-ttu-id="b8eed-126">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [thread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8eed-126">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8eed-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8eed-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b8eed-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8eed-128">Request</span></span>
<span data-ttu-id="b8eed-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8eed-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="b8eed-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8eed-130">Response</span></span>
<span data-ttu-id="b8eed-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8eed-131">The following is an example of the response.</span></span>
><span data-ttu-id="b8eed-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8eed-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
