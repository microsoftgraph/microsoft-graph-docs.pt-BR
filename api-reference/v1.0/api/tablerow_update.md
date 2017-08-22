# <a name="update-tablerow"></a><span data-ttu-id="60eed-101">Atualizar tablerow</span><span class="sxs-lookup"><span data-stu-id="60eed-101">Update tablerow</span></span>

<span data-ttu-id="60eed-102">Atualize as propriedades do objeto tablerow.</span><span class="sxs-lookup"><span data-stu-id="60eed-102">Update the properties of tablerow object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60eed-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60eed-103">Prerequisites</span></span>
<span data-ttu-id="60eed-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="60eed-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="60eed-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60eed-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="60eed-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60eed-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows(<index>)
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="60eed-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="60eed-107">Optional request headers</span></span>
| <span data-ttu-id="60eed-108">Nome</span><span class="sxs-lookup"><span data-stu-id="60eed-108">Name</span></span>       | <span data-ttu-id="60eed-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="60eed-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="60eed-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="60eed-110">Authorization</span></span>  | <span data-ttu-id="60eed-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60eed-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="60eed-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60eed-113">Request body</span></span>
<span data-ttu-id="60eed-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="60eed-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="60eed-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60eed-117">Property</span></span>     | <span data-ttu-id="60eed-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="60eed-118">Type</span></span>   |<span data-ttu-id="60eed-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="60eed-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60eed-120">values</span><span class="sxs-lookup"><span data-stu-id="60eed-120">values</span></span>|<span data-ttu-id="60eed-121">json</span><span class="sxs-lookup"><span data-stu-id="60eed-121">json</span></span>|<span data-ttu-id="60eed-p103">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="60eed-p103">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="60eed-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="60eed-125">Response</span></span>

<span data-ttu-id="60eed-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TableRow](../resources/tablerow.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60eed-126">If successful, this method returns a `200 OK` response code and updated [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60eed-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60eed-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60eed-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60eed-128">Request</span></span>
<span data-ttu-id="60eed-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60eed-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="60eed-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="60eed-130">Response</span></span>
<span data-ttu-id="60eed-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60eed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->