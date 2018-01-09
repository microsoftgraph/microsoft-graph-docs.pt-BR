# <a name="list-conversations"></a><span data-ttu-id="676bd-101">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="676bd-101">List conversations</span></span>
<span data-ttu-id="676bd-102">Recupere a lista de [conversas](../resources/conversation.md) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="676bd-102">Retrieve the list of conversations in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="676bd-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="676bd-103">Permissions</span></span>
<span data-ttu-id="676bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="676bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="676bd-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="676bd-106">Permission type</span></span>      | <span data-ttu-id="676bd-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="676bd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="676bd-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="676bd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="676bd-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="676bd-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="676bd-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="676bd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="676bd-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="676bd-111">Not supported.</span></span>    |
|<span data-ttu-id="676bd-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="676bd-112">Application</span></span> | <span data-ttu-id="676bd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="676bd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="676bd-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="676bd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="676bd-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="676bd-115">Optional query parameters</span></span>
<span data-ttu-id="676bd-116">Este método dá suporte a [Parâmetros de consulta OData](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="676bd-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="676bd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="676bd-117">Request headers</span></span>
| <span data-ttu-id="676bd-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="676bd-118">Header</span></span>       | <span data-ttu-id="676bd-119">Valor</span><span class="sxs-lookup"><span data-stu-id="676bd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="676bd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="676bd-120">Authorization</span></span>  | <span data-ttu-id="676bd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="676bd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="676bd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="676bd-123">Request body</span></span>
<span data-ttu-id="676bd-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="676bd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="676bd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="676bd-125">Response</span></span>
<span data-ttu-id="676bd-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="676bd-126">If successful, this method returns a `200 OK` response code and collection of [Conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="676bd-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="676bd-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="676bd-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="676bd-128">Request</span></span>
<span data-ttu-id="676bd-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="676bd-129">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
#### <a name="response"></a><span data-ttu-id="676bd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="676bd-130">Response</span></span>
<span data-ttu-id="676bd-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="676bd-131">Here is an example of the response.</span></span>
><span data-ttu-id="676bd-132">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="676bd-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="676bd-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="676bd-133">All the properties will be returned from an actual call.</span></span>

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