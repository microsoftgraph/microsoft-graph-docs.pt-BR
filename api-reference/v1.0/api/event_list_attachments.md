# <a name="list-attachments"></a><span data-ttu-id="3b3f2-101">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="3b3f2-101">List attachments</span></span>

<span data-ttu-id="3b3f2-102">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="3b3f2-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b3f2-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b3f2-103">Permissions</span></span>
<span data-ttu-id="3b3f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3b3f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b3f2-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b3f2-106">Permission type</span></span>      | <span data-ttu-id="3b3f2-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b3f2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b3f2-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b3f2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3b3f2-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3b3f2-109">Calendars.Read</span></span>    |
|<span data-ttu-id="3b3f2-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b3f2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b3f2-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3b3f2-111">Calendars.Read</span></span>    |
|<span data-ttu-id="3b3f2-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b3f2-112">Application</span></span> | <span data-ttu-id="3b3f2-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3b3f2-113">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b3f2-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b3f2-114">HTTP request</span></span>
<span data-ttu-id="3b3f2-115">Anexos em um [evento](../resources/event.md) do usuário padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="3b3f2-115">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments
GET /users/{id | userPrincipalName}/events/{id}/attachments

GET /me/calendar/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
GET /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="3b3f2-116">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="3b3f2-116">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="3b3f2-117">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3b3f2-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b3f2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3b3f2-118">Optional query parameters</span></span>
<span data-ttu-id="3b3f2-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3b3f2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3b3f2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3f2-120">Request headers</span></span>
| <span data-ttu-id="3b3f2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3b3f2-121">Name</span></span>       | <span data-ttu-id="3b3f2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b3f2-122">Type</span></span> | <span data-ttu-id="3b3f2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b3f2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3b3f2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b3f2-124">Authorization</span></span>  | <span data-ttu-id="3b3f2-125">string</span><span class="sxs-lookup"><span data-stu-id="3b3f2-125">string</span></span>  | <span data-ttu-id="3b3f2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b3f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b3f2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3f2-128">Request body</span></span>
<span data-ttu-id="3b3f2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b3f2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b3f2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b3f2-130">Response</span></span>

<span data-ttu-id="3b3f2-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b3f2-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b3f2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b3f2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b3f2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3f2-133">Request</span></span>
<span data-ttu-id="3b3f2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b3f2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="3b3f2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b3f2-135">Response</span></span>
<span data-ttu-id="3b3f2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b3f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->