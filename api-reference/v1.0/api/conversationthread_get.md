# <a name="get-conversationthread"></a><span data-ttu-id="4916d-101">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="4916d-101">Get conversationThread</span></span>

<span data-ttu-id="4916d-p101">Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="4916d-p101">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="prerequisites"></a><span data-ttu-id="4916d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4916d-104">Prerequisites</span></span>
<span data-ttu-id="4916d-105">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All; Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="4916d-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All; Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="4916d-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4916d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="4916d-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4916d-107">Optional query parameters</span></span>
<span data-ttu-id="4916d-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4916d-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4916d-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4916d-109">Request headers</span></span>
| <span data-ttu-id="4916d-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4916d-110">Header</span></span>       | <span data-ttu-id="4916d-111">Valor</span><span class="sxs-lookup"><span data-stu-id="4916d-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4916d-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="4916d-112">Authorization</span></span>  | <span data-ttu-id="4916d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4916d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4916d-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4916d-115">Request body</span></span>
<span data-ttu-id="4916d-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4916d-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4916d-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="4916d-117">Response</span></span>

<span data-ttu-id="4916d-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4916d-118">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4916d-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4916d-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4916d-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4916d-120">Request</span></span>
<span data-ttu-id="4916d-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4916d-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="4916d-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="4916d-122">Response</span></span>
<span data-ttu-id="4916d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4916d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
