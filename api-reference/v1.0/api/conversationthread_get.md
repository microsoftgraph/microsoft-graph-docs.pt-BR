# <a name="get-conversationthread"></a><span data-ttu-id="99376-101">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="99376-101">Get conversationThread</span></span>

<span data-ttu-id="99376-p101">Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="99376-p101">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="99376-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="99376-104">Permissions</span></span>
<span data-ttu-id="99376-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="99376-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="99376-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99376-107">Permission type</span></span>      | <span data-ttu-id="99376-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99376-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="99376-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99376-109">Delegated (work or school account)</span></span> | <span data-ttu-id="99376-110">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="99376-110">Group.ReadWrite.All, Group.Read.All</span></span>    | 
|<span data-ttu-id="99376-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99376-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99376-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99376-112">Not supported.</span></span>    | 
|<span data-ttu-id="99376-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99376-113">Application</span></span> | <span data-ttu-id="99376-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="99376-114">Group.ReadWrite.All, Group.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="99376-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99376-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="99376-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99376-116">Optional query parameters</span></span>
<span data-ttu-id="99376-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="99376-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="99376-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99376-118">Request headers</span></span>
| <span data-ttu-id="99376-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99376-119">Header</span></span>       | <span data-ttu-id="99376-120">Valor</span><span class="sxs-lookup"><span data-stu-id="99376-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99376-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="99376-121">Authorization</span></span>  | <span data-ttu-id="99376-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99376-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99376-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99376-124">Request body</span></span>
<span data-ttu-id="99376-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99376-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99376-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="99376-126">Response</span></span>

<span data-ttu-id="99376-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99376-127">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99376-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99376-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99376-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99376-129">Request</span></span>
<span data-ttu-id="99376-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99376-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="99376-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="99376-131">Response</span></span>
<span data-ttu-id="99376-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99376-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
