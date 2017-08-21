# <a name="create-table"></a><span data-ttu-id="0c111-101">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="0c111-101">Create Table</span></span>

<span data-ttu-id="0c111-102">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="0c111-102">Use this API to create a new Table.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c111-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c111-103">Prerequisites</span></span>
<span data-ttu-id="0c111-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="0c111-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="0c111-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c111-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="0c111-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c111-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="0c111-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c111-107">Request headers</span></span>
| <span data-ttu-id="0c111-108">Nome</span><span class="sxs-lookup"><span data-stu-id="0c111-108">Name</span></span>       | <span data-ttu-id="0c111-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c111-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c111-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c111-110">Authorization</span></span>  | <span data-ttu-id="0c111-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c111-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0c111-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c111-113">Request body</span></span>
<span data-ttu-id="0c111-114">No corpo da solicitação, forneça os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0c111-114">In the request body, supply following parameters.</span></span> 

### <a name="request-parameters"></a><span data-ttu-id="0c111-115">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="0c111-115">Request parameters</span></span>
| <span data-ttu-id="0c111-116">Nome</span><span class="sxs-lookup"><span data-stu-id="0c111-116">Name</span></span>           | <span data-ttu-id="0c111-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c111-117">Type</span></span>      |<span data-ttu-id="0c111-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c111-118">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="0c111-119">Endereço</span><span class="sxs-lookup"><span data-stu-id="0c111-119">Address</span></span>  | <span data-ttu-id="0c111-120">string</span><span class="sxs-lookup"><span data-stu-id="0c111-120">string</span></span>| <span data-ttu-id="0c111-p102">Endereço do intervalo. Se você estiver chamando essa API fora do caminho `worksheets/{id or name}/tables/add`, não haverá necessidade do prefixo de nome da planilha no endereço. No entanto, se você a estiver chamando fora do caminho `workbook/tables/add`, forneça então o nome da planilha em que a tabela precisa ser criada (exemplo: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="0c111-p102">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="0c111-124">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="0c111-124">hasHeaders</span></span>  | <span data-ttu-id="0c111-125">booliano</span><span class="sxs-lookup"><span data-stu-id="0c111-125">boolean</span></span>|<span data-ttu-id="0c111-p103">O valor booliano que indica se o intervalo tem rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="0c111-p103">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="0c111-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c111-129">Response</span></span>

<span data-ttu-id="0c111-130">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c111-130">If successful, this method returns `201, Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c111-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c111-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c111-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c111-132">Request</span></span>
<span data-ttu-id="0c111-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c111-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="0c111-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c111-134">Response</span></span>
<span data-ttu-id="0c111-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c111-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
