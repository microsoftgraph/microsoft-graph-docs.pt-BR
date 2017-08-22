# <a name="list-calendars"></a><span data-ttu-id="0625d-101">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="0625d-101">List calendars</span></span>

<span data-ttu-id="0625d-102">Recupera uma lista de calendários que pertencem a um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="0625d-102">Retrieve a list of calendars belonging to a calendar group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0625d-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0625d-103">Prerequisites</span></span>
<span data-ttu-id="0625d-104">Um dos seguintes **escopos** é necessário para executar esta API: _Calendars.Read_</span><span class="sxs-lookup"><span data-stu-id="0625d-104">One of the following **scopes** is required to execute this API: _Calendars.Read_</span></span>
## <a name="http-request"></a><span data-ttu-id="0625d-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0625d-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0625d-106">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="0625d-106">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```
<span data-ttu-id="0625d-107">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0625d-107">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0625d-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0625d-108">Optional query parameters</span></span>
<span data-ttu-id="0625d-109">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0625d-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0625d-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0625d-110">Request headers</span></span>
| <span data-ttu-id="0625d-111">Nome</span><span class="sxs-lookup"><span data-stu-id="0625d-111">Name</span></span>       | <span data-ttu-id="0625d-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="0625d-112">Type</span></span> | <span data-ttu-id="0625d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0625d-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0625d-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="0625d-114">Authorization</span></span>  | <span data-ttu-id="0625d-115">string</span><span class="sxs-lookup"><span data-stu-id="0625d-115">string</span></span>  | <span data-ttu-id="0625d-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0625d-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0625d-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0625d-118">Request body</span></span>
<span data-ttu-id="0625d-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0625d-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0625d-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="0625d-120">Response</span></span>

<span data-ttu-id="0625d-121">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0625d-121">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0625d-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0625d-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0625d-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0625d-123">Request</span></span>
<span data-ttu-id="0625d-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0625d-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```
##### <a name="response"></a><span data-ttu-id="0625d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0625d-125">Response</span></span>
<span data-ttu-id="0625d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0625d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
