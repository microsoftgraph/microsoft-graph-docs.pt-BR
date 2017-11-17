# <a name="update-calendargroup"></a><span data-ttu-id="24ded-101">Atualizar calendargroup</span><span class="sxs-lookup"><span data-stu-id="24ded-101">Update calendargroup</span></span>

<span data-ttu-id="24ded-102">Atualizar as propriedades do objeto calendargroup.</span><span class="sxs-lookup"><span data-stu-id="24ded-102">Update the properties of calendargroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="24ded-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="24ded-103">Permissions</span></span>
<span data-ttu-id="24ded-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24ded-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24ded-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24ded-106">Permission type</span></span>      | <span data-ttu-id="24ded-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24ded-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24ded-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24ded-108">Delegated (work or school account)</span></span> | <span data-ttu-id="24ded-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24ded-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="24ded-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24ded-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24ded-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24ded-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="24ded-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24ded-112">Application</span></span> | <span data-ttu-id="24ded-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24ded-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="24ded-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24ded-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="24ded-115">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="24ded-115">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="24ded-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24ded-116">Request headers</span></span>
| <span data-ttu-id="24ded-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24ded-117">Header</span></span>       | <span data-ttu-id="24ded-118">Valor</span><span class="sxs-lookup"><span data-stu-id="24ded-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24ded-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="24ded-119">Authorization</span></span>  | <span data-ttu-id="24ded-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24ded-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="24ded-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24ded-122">Content-Type</span></span>  | <span data-ttu-id="24ded-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24ded-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="24ded-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24ded-125">Request body</span></span>
<span data-ttu-id="24ded-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="24ded-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="24ded-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24ded-129">Property</span></span>     | <span data-ttu-id="24ded-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="24ded-130">Type</span></span>   |<span data-ttu-id="24ded-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="24ded-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24ded-132">name</span><span class="sxs-lookup"><span data-stu-id="24ded-132">name</span></span>|<span data-ttu-id="24ded-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24ded-133">String</span></span>|<span data-ttu-id="24ded-134">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="24ded-134">The group name.</span></span>|

## <a name="response"></a><span data-ttu-id="24ded-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="24ded-135">Response</span></span>

<span data-ttu-id="24ded-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24ded-136">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24ded-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24ded-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24ded-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24ded-138">Request</span></span>
<span data-ttu-id="24ded-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24ded-139">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="24ded-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="24ded-140">Response</span></span>
<span data-ttu-id="24ded-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24ded-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
