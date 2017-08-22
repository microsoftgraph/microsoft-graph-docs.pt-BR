# <a name="update-tablecolumn"></a><span data-ttu-id="ee986-101">Atualizar tablecolumn</span><span class="sxs-lookup"><span data-stu-id="ee986-101">Update tablecolumn</span></span>

<span data-ttu-id="ee986-102">Atualize as propriedades do objeto tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="ee986-102">Update the properties of tablecolumn object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee986-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee986-103">Prerequisites</span></span>
<span data-ttu-id="ee986-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="ee986-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="ee986-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee986-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="ee986-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee986-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ee986-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ee986-107">Optional request headers</span></span>
| <span data-ttu-id="ee986-108">Nome</span><span class="sxs-lookup"><span data-stu-id="ee986-108">Name</span></span>       | <span data-ttu-id="ee986-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee986-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ee986-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee986-110">Authorization</span></span>  | <span data-ttu-id="ee986-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee986-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ee986-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee986-113">Request body</span></span>
<span data-ttu-id="ee986-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ee986-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ee986-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee986-117">Property</span></span>     | <span data-ttu-id="ee986-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee986-118">Type</span></span>   |<span data-ttu-id="ee986-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee986-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee986-120">values</span><span class="sxs-lookup"><span data-stu-id="ee986-120">values</span></span>|<span data-ttu-id="ee986-121">json</span><span class="sxs-lookup"><span data-stu-id="ee986-121">json</span></span>|<span data-ttu-id="ee986-p103">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="ee986-p103">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="ee986-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee986-125">Response</span></span>

<span data-ttu-id="ee986-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TableColumn](../resources/tablecolumn.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee986-126">If successful, this method returns a `200 OK` response code and updated [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee986-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee986-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee986-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee986-128">Request</span></span>
<span data-ttu-id="ee986-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee986-129">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ee986-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee986-130">Response</span></span>
<span data-ttu-id="ee986-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee986-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
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