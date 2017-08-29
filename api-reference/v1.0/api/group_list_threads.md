# <a name="list-threads"></a><span data-ttu-id="5cbfd-101">Listar threads</span><span class="sxs-lookup"><span data-stu-id="5cbfd-101">List threads</span></span>

<span data-ttu-id="5cbfd-102">Obtenha todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="5cbfd-102">Get all the threads of a group.</span></span>

<span data-ttu-id="5cbfd-103">Observação: Você também pode [obter todos os threads de uma conversa](conversation_list_threads.md).</span><span class="sxs-lookup"><span data-stu-id="5cbfd-103">Note: You can also [get all the threads of a conversation](conversation_list_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5cbfd-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="5cbfd-104">Permissions</span></span>
<span data-ttu-id="5cbfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5cbfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5cbfd-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cbfd-107">Permission type</span></span>      | <span data-ttu-id="5cbfd-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5cbfd-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cbfd-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cbfd-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5cbfd-110">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cbfd-110">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5cbfd-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cbfd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cbfd-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cbfd-112">Not supported.</span></span>    |
|<span data-ttu-id="5cbfd-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cbfd-113">Application</span></span> | <span data-ttu-id="5cbfd-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cbfd-114">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cbfd-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cbfd-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5cbfd-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5cbfd-116">Optional query parameters</span></span>
<span data-ttu-id="5cbfd-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5cbfd-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5cbfd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cbfd-118">Request headers</span></span>
| <span data-ttu-id="5cbfd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5cbfd-119">Header</span></span>       | <span data-ttu-id="5cbfd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5cbfd-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5cbfd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cbfd-121">Authorization</span></span>  | <span data-ttu-id="5cbfd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cbfd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cbfd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cbfd-124">Request body</span></span>
<span data-ttu-id="5cbfd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5cbfd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cbfd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cbfd-126">Response</span></span>

<span data-ttu-id="5cbfd-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cbfd-127">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5cbfd-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cbfd-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cbfd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cbfd-129">Request</span></span>
<span data-ttu-id="5cbfd-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cbfd-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="5cbfd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cbfd-131">Response</span></span>
<span data-ttu-id="5cbfd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5cbfd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
