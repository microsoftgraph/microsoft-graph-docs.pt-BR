# <a name="update-table"></a><span data-ttu-id="e46d0-101">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="e46d0-101">Update table</span></span>

<span data-ttu-id="e46d0-102">Atualize as propriedades do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="e46d0-102">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e46d0-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e46d0-103">Permissions</span></span>
<span data-ttu-id="e46d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e46d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e46d0-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e46d0-106">Permission type</span></span>      | <span data-ttu-id="e46d0-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e46d0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e46d0-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e46d0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e46d0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e46d0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e46d0-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e46d0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e46d0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e46d0-111">Not supported.</span></span>    |
|<span data-ttu-id="e46d0-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e46d0-112">Application</span></span> | <span data-ttu-id="e46d0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e46d0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e46d0-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e46d0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e46d0-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e46d0-115">Optional request headers</span></span>
| <span data-ttu-id="e46d0-116">Nome</span><span class="sxs-lookup"><span data-stu-id="e46d0-116">Name</span></span>       | <span data-ttu-id="e46d0-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="e46d0-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e46d0-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="e46d0-118">Authorization</span></span>  | <span data-ttu-id="e46d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e46d0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e46d0-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e46d0-121">Request body</span></span>
<span data-ttu-id="e46d0-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e46d0-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e46d0-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e46d0-125">Property</span></span>     | <span data-ttu-id="e46d0-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e46d0-126">Type</span></span>   |<span data-ttu-id="e46d0-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e46d0-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e46d0-128">name</span><span class="sxs-lookup"><span data-stu-id="e46d0-128">name</span></span>|<span data-ttu-id="e46d0-129">string</span><span class="sxs-lookup"><span data-stu-id="e46d0-129">string</span></span>|<span data-ttu-id="e46d0-130">Nome da tabela.</span><span class="sxs-lookup"><span data-stu-id="e46d0-130">Name of the table.</span></span>|
|<span data-ttu-id="e46d0-131">showHeaders</span><span class="sxs-lookup"><span data-stu-id="e46d0-131">showHeaders</span></span>|<span data-ttu-id="e46d0-132">booliano</span><span class="sxs-lookup"><span data-stu-id="e46d0-132">boolean</span></span>|<span data-ttu-id="e46d0-p104">Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="e46d0-p104">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="e46d0-135">showTotals</span><span class="sxs-lookup"><span data-stu-id="e46d0-135">showTotals</span></span>|<span data-ttu-id="e46d0-136">booliano</span><span class="sxs-lookup"><span data-stu-id="e46d0-136">boolean</span></span>|<span data-ttu-id="e46d0-p105">Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.</span><span class="sxs-lookup"><span data-stu-id="e46d0-p105">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="e46d0-139">style</span><span class="sxs-lookup"><span data-stu-id="e46d0-139">style</span></span>|<span data-ttu-id="e46d0-140">string</span><span class="sxs-lookup"><span data-stu-id="e46d0-140">string</span></span>|<span data-ttu-id="e46d0-p106">Valor da constante que representa o estilo de Tabela. Os valores possíveis são: TableStyleLight1 a TableStyleLight21, TableStyleMedium1 a TableStyleMedium28, TableStyleStyleDark1 a TableStyleStyleDark11. Também é possível usar um estilo definido pelo usuário que esteja presente na planilha.</span><span class="sxs-lookup"><span data-stu-id="e46d0-p106">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="e46d0-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e46d0-144">Response</span></span>

<span data-ttu-id="e46d0-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Table](../resources/table.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e46d0-145">If successful, this method returns a `200 OK` response code and updated [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e46d0-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e46d0-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e46d0-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e46d0-147">Request</span></span>
<span data-ttu-id="e46d0-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e46d0-148">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e46d0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e46d0-149">Response</span></span>
<span data-ttu-id="e46d0-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e46d0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
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
