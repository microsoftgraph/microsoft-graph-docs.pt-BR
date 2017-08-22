# <a name="list-events"></a><span data-ttu-id="00d02-101">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="00d02-101">List events</span></span>

<span data-ttu-id="00d02-102">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="00d02-102">Retrieve a list of [event](../resources/event.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00d02-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00d02-103">Prerequisites</span></span>
<span data-ttu-id="00d02-104">Um dos seguintes **escopos** é obrigatório para executar esta API: _Group.Read.All_ ou _Group.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="00d02-104">One of the following **scopes** is required to execute this API: _Group.Read.All_ or _Group.ReadWrite.All_</span></span>
## <a name="http-request"></a><span data-ttu-id="00d02-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00d02-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="00d02-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00d02-106">Optional query parameters</span></span>
<span data-ttu-id="00d02-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00d02-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="00d02-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00d02-108">Request headers</span></span>
| <span data-ttu-id="00d02-109">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00d02-109">Header</span></span>       | <span data-ttu-id="00d02-110">Valor</span><span class="sxs-lookup"><span data-stu-id="00d02-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00d02-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="00d02-111">Authorization</span></span>  | <span data-ttu-id="00d02-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00d02-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00d02-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00d02-114">Request body</span></span>
<span data-ttu-id="00d02-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00d02-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00d02-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="00d02-116">Response</span></span>

<span data-ttu-id="00d02-117">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00d02-117">If successful, this method returns a `200 OK` response code and a collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00d02-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00d02-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00d02-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00d02-119">Request</span></span>
<span data-ttu-id="00d02-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00d02-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/events
```
##### <a name="response"></a><span data-ttu-id="00d02-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="00d02-121">Response</span></span>
<span data-ttu-id="00d02-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00d02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
