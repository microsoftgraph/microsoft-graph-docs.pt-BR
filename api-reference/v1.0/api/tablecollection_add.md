# <a name="tablecollection-add"></a><span data-ttu-id="0e521-101">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="0e521-101">TableCollection: add</span></span>

<span data-ttu-id="0e521-p101">Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.</span><span class="sxs-lookup"><span data-stu-id="0e521-p101">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e521-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e521-105">Prerequisites</span></span>
<span data-ttu-id="0e521-106">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="0e521-106">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="0e521-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e521-107">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="0e521-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e521-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="0e521-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e521-109">Request headers</span></span>
| <span data-ttu-id="0e521-110">Nome</span><span class="sxs-lookup"><span data-stu-id="0e521-110">Name</span></span>       | <span data-ttu-id="0e521-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e521-111">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e521-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e521-112">Authorization</span></span>  | <span data-ttu-id="0e521-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e521-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0e521-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e521-115">Request body</span></span>
<span data-ttu-id="0e521-116">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e521-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e521-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0e521-117">Parameter</span></span>    | <span data-ttu-id="0e521-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e521-118">Type</span></span>   |<span data-ttu-id="0e521-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e521-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e521-120">address</span><span class="sxs-lookup"><span data-stu-id="0e521-120">address</span></span>|<span data-ttu-id="0e521-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e521-121">string</span></span>|<span data-ttu-id="0e521-p103">Endereço ou nome do objeto de intervalo que representa a fonte de dados. Se o endereço não contiver o nome de uma planilha, a folha ativa no momento será usada.</span><span class="sxs-lookup"><span data-stu-id="0e521-p103">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="0e521-124">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="0e521-124">hasHeaders</span></span>|<span data-ttu-id="0e521-125">booliano</span><span class="sxs-lookup"><span data-stu-id="0e521-125">boolean</span></span>|<span data-ttu-id="0e521-p104">Valor booliano que indica se os dados que estão sendo importados têm rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="0e521-p104">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="0e521-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e521-129">Response</span></span>

<span data-ttu-id="0e521-130">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e521-130">If successful, this method returns `200, OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e521-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e521-131">Example</span></span>
<span data-ttu-id="0e521-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0e521-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e521-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e521-133">Request</span></span>
<span data-ttu-id="0e521-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e521-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="0e521-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e521-135">Response</span></span>
<span data-ttu-id="0e521-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e521-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
