# <a name="list-conversations"></a><span data-ttu-id="b6f23-101">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="b6f23-101">List conversations</span></span>

<span data-ttu-id="b6f23-102">Recupere a lista de conversas desse grupo.</span><span class="sxs-lookup"><span data-stu-id="b6f23-102">Retrieve the list of conversations in this group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6f23-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6f23-103">Prerequisites</span></span>
<span data-ttu-id="b6f23-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Group.Read.All* ou *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="b6f23-104">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="b6f23-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f23-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6f23-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6f23-106">Optional query parameters</span></span>
<span data-ttu-id="b6f23-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f23-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b6f23-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f23-108">Request headers</span></span>
| <span data-ttu-id="b6f23-109">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6f23-109">Header</span></span>       | <span data-ttu-id="b6f23-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b6f23-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b6f23-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6f23-111">Authorization</span></span>  | <span data-ttu-id="b6f23-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6f23-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b6f23-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f23-114">Request body</span></span>
<span data-ttu-id="b6f23-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6f23-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6f23-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f23-116">Response</span></span>

<span data-ttu-id="b6f23-117">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f23-117">If successful, this method returns a `200 OK` response code and collection of [Conversation](../resources/conversation.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6f23-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6f23-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6f23-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f23-119">Request</span></span>
<span data-ttu-id="b6f23-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6f23-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
##### <a name="response"></a><span data-ttu-id="b6f23-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f23-121">Response</span></span>
<span data-ttu-id="b6f23-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6f23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->