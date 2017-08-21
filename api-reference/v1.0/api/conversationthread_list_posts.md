# <a name="list-posts"></a><span data-ttu-id="fc3ff-101">Listar postagens</span><span class="sxs-lookup"><span data-stu-id="fc3ff-101">List posts</span></span>

<span data-ttu-id="fc3ff-p101">Obtenha as postagens do thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="fc3ff-p101">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc3ff-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc3ff-104">Prerequisites</span></span>
<span data-ttu-id="fc3ff-105">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All; Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="fc3ff-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All; Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="fc3ff-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc3ff-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="fc3ff-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc3ff-107">Optional query parameters</span></span>
<span data-ttu-id="fc3ff-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc3ff-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fc3ff-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3ff-109">Request headers</span></span>
| <span data-ttu-id="fc3ff-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc3ff-110">Header</span></span>       | <span data-ttu-id="fc3ff-111">Valor</span><span class="sxs-lookup"><span data-stu-id="fc3ff-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc3ff-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc3ff-112">Authorization</span></span>  | <span data-ttu-id="fc3ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc3ff-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc3ff-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3ff-115">Request body</span></span>
<span data-ttu-id="fc3ff-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc3ff-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc3ff-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3ff-117">Response</span></span>

<span data-ttu-id="fc3ff-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc3ff-118">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc3ff-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc3ff-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc3ff-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3ff-120">Request</span></span>
<span data-ttu-id="fc3ff-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc3ff-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="fc3ff-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3ff-122">Response</span></span>
<span data-ttu-id="fc3ff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc3ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
  "value": [
    {
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "receivedDateTime": "datetime-value",
      "hasAttachments": true,
      "from": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "conversationThreadId": "conversationThreadId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
