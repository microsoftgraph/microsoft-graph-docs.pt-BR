# <a name="list-posts"></a><span data-ttu-id="40252-101">Listar postagens</span><span class="sxs-lookup"><span data-stu-id="40252-101">List posts</span></span>

<span data-ttu-id="40252-p101">Obtenha as postagens do thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="40252-p101">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="40252-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="40252-104">Permissions</span></span>
<span data-ttu-id="40252-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="40252-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="40252-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40252-107">Permission type</span></span>      | <span data-ttu-id="40252-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40252-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40252-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40252-109">Delegated (work or school account)</span></span> | <span data-ttu-id="40252-110">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="40252-110">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="40252-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40252-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40252-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40252-112">Not supported.</span></span>    |
|<span data-ttu-id="40252-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40252-113">Application</span></span> | <span data-ttu-id="40252-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="40252-114">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40252-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40252-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="40252-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40252-116">Optional query parameters</span></span>
<span data-ttu-id="40252-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40252-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="40252-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40252-118">Request headers</span></span>
| <span data-ttu-id="40252-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40252-119">Header</span></span>       | <span data-ttu-id="40252-120">Valor</span><span class="sxs-lookup"><span data-stu-id="40252-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40252-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="40252-121">Authorization</span></span>  | <span data-ttu-id="40252-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40252-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40252-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40252-124">Request body</span></span>
<span data-ttu-id="40252-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40252-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40252-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="40252-126">Response</span></span>

<span data-ttu-id="40252-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40252-127">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40252-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40252-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40252-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40252-129">Request</span></span>
<span data-ttu-id="40252-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40252-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="40252-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="40252-131">Response</span></span>
<span data-ttu-id="40252-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40252-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
