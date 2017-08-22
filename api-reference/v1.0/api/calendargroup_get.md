# <a name="get-calendargroup"></a><span data-ttu-id="f5f0b-101">Obter calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f5f0b-101">Get calendarGroup</span></span>

<span data-ttu-id="f5f0b-102">Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-102">Retrieve the properties and relationships of a calendar group object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5f0b-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5f0b-103">Prerequisites</span></span>
<span data-ttu-id="f5f0b-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.Read*</span><span class="sxs-lookup"><span data-stu-id="f5f0b-104">One of the following **scopes** is required to execute this API: *Calendars.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="f5f0b-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5f0b-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f5f0b-106">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-106">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5f0b-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5f0b-107">Optional query parameters</span></span>
<span data-ttu-id="f5f0b-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f5f0b-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f0b-109">Request headers</span></span>
| <span data-ttu-id="f5f0b-110">Nome</span><span class="sxs-lookup"><span data-stu-id="f5f0b-110">Name</span></span>       | <span data-ttu-id="f5f0b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5f0b-111">Type</span></span> | <span data-ttu-id="f5f0b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5f0b-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5f0b-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5f0b-113">Authorization</span></span>  | <span data-ttu-id="f5f0b-114">string</span><span class="sxs-lookup"><span data-stu-id="f5f0b-114">string</span></span>  | <span data-ttu-id="f5f0b-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5f0b-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f0b-117">Request body</span></span>
<span data-ttu-id="f5f0b-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5f0b-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f0b-119">Response</span></span>

<span data-ttu-id="f5f0b-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-120">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5f0b-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5f0b-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5f0b-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f0b-122">Request</span></span>
<span data-ttu-id="f5f0b-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="f5f0b-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f0b-124">Response</span></span>
<span data-ttu-id="f5f0b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
