# <a name="get-post"></a><span data-ttu-id="91f3c-101">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="91f3c-101">Get post</span></span>

<span data-ttu-id="91f3c-p101">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="91f3c-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="91f3c-104">Como o recurso **post** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **post**.</span><span class="sxs-lookup"><span data-stu-id="91f3c-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="91f3c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="91f3c-105">Permissions</span></span>
<span data-ttu-id="91f3c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="91f3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="91f3c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91f3c-108">Permission type</span></span>      | <span data-ttu-id="91f3c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91f3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91f3c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91f3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91f3c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f3c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="91f3c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91f3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91f3c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91f3c-113">Not supported.</span></span>    |
|<span data-ttu-id="91f3c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91f3c-114">Application</span></span> | <span data-ttu-id="91f3c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f3c-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91f3c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91f3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91f3c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="91f3c-117">Optional query parameters</span></span>
<span data-ttu-id="91f3c-118">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="91f3c-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="91f3c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91f3c-119">Request headers</span></span>
| <span data-ttu-id="91f3c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91f3c-120">Header</span></span>       | <span data-ttu-id="91f3c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="91f3c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91f3c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="91f3c-122">Authorization</span></span>  | <span data-ttu-id="91f3c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91f3c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91f3c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91f3c-125">Request body</span></span>
<span data-ttu-id="91f3c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91f3c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91f3c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f3c-127">Response</span></span>

<span data-ttu-id="91f3c-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91f3c-128">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91f3c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91f3c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91f3c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91f3c-130">Request</span></span>
<span data-ttu-id="91f3c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91f3c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="91f3c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f3c-132">Response</span></span>
<span data-ttu-id="91f3c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91f3c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="91f3c-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="91f3c-136">See also</span></span>

- [<span data-ttu-id="91f3c-137">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="91f3c-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="91f3c-138">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="91f3c-138">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
