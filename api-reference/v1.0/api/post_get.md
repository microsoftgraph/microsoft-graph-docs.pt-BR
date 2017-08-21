# <a name="get-post"></a><span data-ttu-id="b1e82-101">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="b1e82-101">Get post</span></span>

<span data-ttu-id="b1e82-p101">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="b1e82-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="b1e82-104">Como o recurso **post** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **post**.</span><span class="sxs-lookup"><span data-stu-id="b1e82-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1e82-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1e82-105">Prerequisites</span></span>
<span data-ttu-id="b1e82-106">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="b1e82-106">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="b1e82-107">*Group.Read.All*, *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="b1e82-107">*Group.Read.All*, *Group.Readwrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="b1e82-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1e82-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1e82-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1e82-109">Optional query parameters</span></span>
<span data-ttu-id="b1e82-110">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1e82-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1e82-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e82-111">Request headers</span></span>
| <span data-ttu-id="b1e82-112">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1e82-112">Header</span></span>       | <span data-ttu-id="b1e82-113">Valor</span><span class="sxs-lookup"><span data-stu-id="b1e82-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1e82-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1e82-114">Authorization</span></span>  | <span data-ttu-id="b1e82-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1e82-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1e82-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e82-117">Request body</span></span>
<span data-ttu-id="b1e82-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1e82-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1e82-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1e82-119">Response</span></span>

<span data-ttu-id="b1e82-120">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1e82-120">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1e82-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1e82-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1e82-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e82-122">Request</span></span>
<span data-ttu-id="b1e82-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1e82-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="b1e82-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1e82-124">Response</span></span>
<span data-ttu-id="b1e82-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1e82-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

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
  }
}
```

## <a name="see-also"></a><span data-ttu-id="b1e82-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="b1e82-128">See also</span></span>

- [<span data-ttu-id="b1e82-129">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="b1e82-129">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="b1e82-130">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="b1e82-130">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
