# <a name="update-tablecolumn"></a><span data-ttu-id="3d8d4-101">Atualizar tablecolumn</span><span class="sxs-lookup"><span data-stu-id="3d8d4-101">Update tablecolumn</span></span>

<span data-ttu-id="3d8d4-102">Atualize as propriedades do objeto tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-102">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d8d4-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d8d4-103">Permissions</span></span>
<span data-ttu-id="3d8d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d8d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3d8d4-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d8d4-106">Permission type</span></span>      | <span data-ttu-id="3d8d4-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d8d4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d8d4-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d8d4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3d8d4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d8d4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3d8d4-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d8d4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d8d4-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-111">Not supported.</span></span>    |
|<span data-ttu-id="3d8d4-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d8d4-112">Application</span></span> | <span data-ttu-id="3d8d4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d8d4-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d8d4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3d8d4-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="3d8d4-115">Optional request headers</span></span>
| <span data-ttu-id="3d8d4-116">Nome</span><span class="sxs-lookup"><span data-stu-id="3d8d4-116">Name</span></span>       | <span data-ttu-id="3d8d4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d8d4-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3d8d4-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d8d4-118">Authorization</span></span>  | <span data-ttu-id="3d8d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d8d4-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3d8d4-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3d8d4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d8d4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d8d4-124">Request body</span></span>
<span data-ttu-id="3d8d4-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3d8d4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d8d4-128">Property</span></span>     | <span data-ttu-id="3d8d4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d8d4-129">Type</span></span>   |<span data-ttu-id="3d8d4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d8d4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d8d4-131">values</span><span class="sxs-lookup"><span data-stu-id="3d8d4-131">values</span></span>|<span data-ttu-id="3d8d4-132">Json</span><span class="sxs-lookup"><span data-stu-id="3d8d4-132">Json</span></span>|<span data-ttu-id="3d8d4-p105">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="3d8d4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d8d4-136">Response</span></span>

<span data-ttu-id="3d8d4-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [WorkbookTableColumn](../resources/tablecolumn.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-137">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d8d4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d8d4-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d8d4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d8d4-139">Request</span></span>
<span data-ttu-id="3d8d4-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="3d8d4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d8d4-141">Response</span></span>
<span data-ttu-id="3d8d4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d8d4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->