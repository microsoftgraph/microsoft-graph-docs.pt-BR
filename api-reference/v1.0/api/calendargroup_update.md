# <a name="update-calendargroup"></a><span data-ttu-id="59fcc-101">Atualizar calendargroup</span><span class="sxs-lookup"><span data-stu-id="59fcc-101">Update calendargroup</span></span>

<span data-ttu-id="59fcc-102">Atualiza as propriedades do objeto calendargroup.</span><span class="sxs-lookup"><span data-stu-id="59fcc-102">Update the properties of calendargroup object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59fcc-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59fcc-103">Prerequisites</span></span>
<span data-ttu-id="59fcc-104">Um dos seguintes **escopos** é necessário para executar esta API: _Calendars.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="59fcc-104">One of the following **scopes** is required to execute this API: _Calendars.ReadWrite_</span></span>
## <a name="http-request"></a><span data-ttu-id="59fcc-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59fcc-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="59fcc-106">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="59fcc-106">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="59fcc-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59fcc-107">Request headers</span></span>
| <span data-ttu-id="59fcc-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59fcc-108">Header</span></span>       | <span data-ttu-id="59fcc-109">Valor</span><span class="sxs-lookup"><span data-stu-id="59fcc-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59fcc-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="59fcc-110">Authorization</span></span>  | <span data-ttu-id="59fcc-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59fcc-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59fcc-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59fcc-113">Content-Type</span></span>  | <span data-ttu-id="59fcc-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59fcc-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59fcc-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59fcc-116">Request body</span></span>
<span data-ttu-id="59fcc-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="59fcc-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59fcc-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59fcc-120">Property</span></span>     | <span data-ttu-id="59fcc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="59fcc-121">Type</span></span>   |<span data-ttu-id="59fcc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="59fcc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59fcc-123">name</span><span class="sxs-lookup"><span data-stu-id="59fcc-123">name</span></span>|<span data-ttu-id="59fcc-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fcc-124">String</span></span>|<span data-ttu-id="59fcc-125">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="59fcc-125">The group name.</span></span>|

## <a name="response"></a><span data-ttu-id="59fcc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="59fcc-126">Response</span></span>

<span data-ttu-id="59fcc-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59fcc-127">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59fcc-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59fcc-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59fcc-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59fcc-129">Request</span></span>
<span data-ttu-id="59fcc-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59fcc-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="59fcc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="59fcc-131">Response</span></span>
<span data-ttu-id="59fcc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59fcc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
