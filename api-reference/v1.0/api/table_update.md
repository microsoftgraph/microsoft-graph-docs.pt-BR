# <a name="update-table"></a><span data-ttu-id="32624-101">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="32624-101">Update table</span></span>

<span data-ttu-id="32624-102">Atualize as propriedades do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="32624-102">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="32624-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="32624-103">Permissions</span></span>
<span data-ttu-id="32624-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="32624-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32624-106">Permission type</span></span>      | <span data-ttu-id="32624-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32624-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32624-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32624-108">Delegated (work or school account)</span></span> | <span data-ttu-id="32624-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32624-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="32624-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32624-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32624-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32624-111">Not supported.</span></span>    |
|<span data-ttu-id="32624-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32624-112">Application</span></span> | <span data-ttu-id="32624-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32624-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32624-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32624-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="32624-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="32624-115">Optional request headers</span></span>
| <span data-ttu-id="32624-116">Nome</span><span class="sxs-lookup"><span data-stu-id="32624-116">Name</span></span>       | <span data-ttu-id="32624-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="32624-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="32624-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="32624-118">Authorization</span></span>  | <span data-ttu-id="32624-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32624-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32624-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="32624-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="32624-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="32624-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32624-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32624-124">Request body</span></span>
<span data-ttu-id="32624-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="32624-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="32624-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32624-128">Property</span></span>     | <span data-ttu-id="32624-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="32624-129">Type</span></span>   |<span data-ttu-id="32624-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="32624-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32624-131">name</span><span class="sxs-lookup"><span data-stu-id="32624-131">name</span></span>|<span data-ttu-id="32624-132">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="32624-132">string</span></span>|<span data-ttu-id="32624-133">Nome da tabela.</span><span class="sxs-lookup"><span data-stu-id="32624-133">Name of the table.</span></span>|
|<span data-ttu-id="32624-134">showHeaders</span><span class="sxs-lookup"><span data-stu-id="32624-134">showHeaders</span></span>|<span data-ttu-id="32624-135">booliano</span><span class="sxs-lookup"><span data-stu-id="32624-135">boolean</span></span>|<span data-ttu-id="32624-p105">Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="32624-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="32624-138">showTotals</span><span class="sxs-lookup"><span data-stu-id="32624-138">showTotals</span></span>|<span data-ttu-id="32624-139">booliano</span><span class="sxs-lookup"><span data-stu-id="32624-139">boolean</span></span>|<span data-ttu-id="32624-p106">Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.</span><span class="sxs-lookup"><span data-stu-id="32624-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="32624-142">style</span><span class="sxs-lookup"><span data-stu-id="32624-142">style</span></span>|<span data-ttu-id="32624-143">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="32624-143">string</span></span>|<span data-ttu-id="32624-144">Valor constante que representa o estilo de tabela.</span><span class="sxs-lookup"><span data-stu-id="32624-144">Constant value that represents the Table style.</span></span> <span data-ttu-id="32624-145">Os valores possíveis são: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span><span class="sxs-lookup"><span data-stu-id="32624-145">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="32624-146">Também pode ser especificado um estilo personalizado definido pelo usuário presente na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="32624-146">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="32624-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="32624-147">Response</span></span>

<span data-ttu-id="32624-148">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [WorkbookTable](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32624-148">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32624-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32624-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32624-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32624-150">Request</span></span>
<span data-ttu-id="32624-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32624-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="32624-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="32624-152">Response</span></span>
<span data-ttu-id="32624-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32624-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
