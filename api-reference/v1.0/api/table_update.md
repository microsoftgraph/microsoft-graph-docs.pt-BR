# <a name="update-table"></a><span data-ttu-id="59f44-101">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="59f44-101">Update table</span></span>

<span data-ttu-id="59f44-102">Atualize as propriedades do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="59f44-102">Update the properties of table object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59f44-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59f44-103">Prerequisites</span></span>
<span data-ttu-id="59f44-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="59f44-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="59f44-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59f44-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="59f44-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59f44-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="59f44-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="59f44-107">Optional request headers</span></span>
| <span data-ttu-id="59f44-108">Nome</span><span class="sxs-lookup"><span data-stu-id="59f44-108">Name</span></span>       | <span data-ttu-id="59f44-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f44-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="59f44-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="59f44-110">Authorization</span></span>  | <span data-ttu-id="59f44-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59f44-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="59f44-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59f44-113">Request body</span></span>
<span data-ttu-id="59f44-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="59f44-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59f44-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59f44-117">Property</span></span>     | <span data-ttu-id="59f44-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="59f44-118">Type</span></span>   |<span data-ttu-id="59f44-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f44-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59f44-120">name</span><span class="sxs-lookup"><span data-stu-id="59f44-120">name</span></span>|<span data-ttu-id="59f44-121">string</span><span class="sxs-lookup"><span data-stu-id="59f44-121">string</span></span>|<span data-ttu-id="59f44-122">Nome da tabela.</span><span class="sxs-lookup"><span data-stu-id="59f44-122">Name of the table.</span></span>|
|<span data-ttu-id="59f44-123">showHeaders</span><span class="sxs-lookup"><span data-stu-id="59f44-123">showHeaders</span></span>|<span data-ttu-id="59f44-124">booliano</span><span class="sxs-lookup"><span data-stu-id="59f44-124">boolean</span></span>|<span data-ttu-id="59f44-p103">Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="59f44-p103">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="59f44-127">showTotals</span><span class="sxs-lookup"><span data-stu-id="59f44-127">showTotals</span></span>|<span data-ttu-id="59f44-128">booliano</span><span class="sxs-lookup"><span data-stu-id="59f44-128">boolean</span></span>|<span data-ttu-id="59f44-p104">Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.</span><span class="sxs-lookup"><span data-stu-id="59f44-p104">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="59f44-131">style</span><span class="sxs-lookup"><span data-stu-id="59f44-131">style</span></span>|<span data-ttu-id="59f44-132">string</span><span class="sxs-lookup"><span data-stu-id="59f44-132">string</span></span>|<span data-ttu-id="59f44-p105">Valor da constante que representa o estilo de Tabela. Os valores possíveis são: TableStyleLight1 a TableStyleLight21, TableStyleMedium1 a TableStyleMedium28, TableStyleStyleDark1 a TableStyleStyleDark11. Também é possível usar um estilo definido pelo usuário que esteja presente na planilha.</span><span class="sxs-lookup"><span data-stu-id="59f44-p105">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="59f44-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f44-136">Response</span></span>

<span data-ttu-id="59f44-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Table](../resources/table.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59f44-137">If successful, this method returns a `200 OK` response code and updated [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59f44-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59f44-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59f44-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59f44-139">Request</span></span>
<span data-ttu-id="59f44-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59f44-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="59f44-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f44-141">Response</span></span>
<span data-ttu-id="59f44-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59f44-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
