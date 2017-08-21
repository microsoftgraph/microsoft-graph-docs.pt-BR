# <a name="create-table"></a><span data-ttu-id="addec-101">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="addec-101">Create Table</span></span>

<span data-ttu-id="addec-102">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="addec-102">Use this API to create a new Table.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="addec-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="addec-103">Prerequisites</span></span>
<span data-ttu-id="addec-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="addec-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="addec-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="addec-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="addec-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="addec-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="addec-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="addec-107">Request headers</span></span>
| <span data-ttu-id="addec-108">Nome</span><span class="sxs-lookup"><span data-stu-id="addec-108">Name</span></span>       | <span data-ttu-id="addec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="addec-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="addec-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="addec-110">Authorization</span></span>  | <span data-ttu-id="addec-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="addec-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="addec-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="addec-113">Request body</span></span>
<span data-ttu-id="addec-114">No corpo da solicitação, forneça uma representação JSON do objeto [Table](../resources/table.md).</span><span class="sxs-lookup"><span data-stu-id="addec-114">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="addec-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="addec-115">Response</span></span>

<span data-ttu-id="addec-116">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="addec-116">If successful, this method returns `201, Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="addec-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="addec-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="addec-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="addec-118">Request</span></span>
<span data-ttu-id="addec-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="addec-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "id": 99,
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
<span data-ttu-id="addec-120">No corpo da solicitação, forneça uma representação JSON do objeto [Table](../resources/table.md).</span><span class="sxs-lookup"><span data-stu-id="addec-120">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="addec-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="addec-121">Response</span></span>
<span data-ttu-id="addec-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="addec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
