# <a name="list-threads"></a><span data-ttu-id="9419a-101">Listar threads</span><span class="sxs-lookup"><span data-stu-id="9419a-101">List threads</span></span>

<span data-ttu-id="9419a-102">Obtenha todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="9419a-102">Get all the threads of a group.</span></span>

<span data-ttu-id="9419a-103">Observação: Você também pode [obter todos os threads de uma conversa](conversation_list_threads.md).</span><span class="sxs-lookup"><span data-stu-id="9419a-103">Note: You can also [get all the threads of a conversation](conversation_list_threads.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9419a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9419a-104">Prerequisites</span></span>
<span data-ttu-id="9419a-105">Um dos seguintes **escopos** é obrigatório para executar esta API:  *Group.Read.All* ou *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="9419a-105">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="9419a-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9419a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9419a-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9419a-107">Optional query parameters</span></span>
<span data-ttu-id="9419a-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9419a-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9419a-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9419a-109">Request headers</span></span>
| <span data-ttu-id="9419a-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9419a-110">Header</span></span>       | <span data-ttu-id="9419a-111">Valor</span><span class="sxs-lookup"><span data-stu-id="9419a-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9419a-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="9419a-112">Authorization</span></span>  | <span data-ttu-id="9419a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9419a-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9419a-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9419a-115">Request body</span></span>
<span data-ttu-id="9419a-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9419a-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9419a-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="9419a-117">Response</span></span>

<span data-ttu-id="9419a-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9419a-118">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9419a-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9419a-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9419a-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9419a-120">Request</span></span>
<span data-ttu-id="9419a-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9419a-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="9419a-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="9419a-122">Response</span></span>
<span data-ttu-id="9419a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9419a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
