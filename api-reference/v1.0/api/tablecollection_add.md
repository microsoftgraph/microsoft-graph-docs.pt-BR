# <a name="tablecollection-add"></a><span data-ttu-id="b8091-101">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="b8091-101">TableCollection: add</span></span>

<span data-ttu-id="b8091-p101">Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.</span><span class="sxs-lookup"><span data-stu-id="b8091-p101">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="b8091-105">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="b8091-105">Error Handling</span></span>

<span data-ttu-id="b8091-106">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="b8091-106">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="b8091-107">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8091-107">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8091-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8091-108">Permissions</span></span>
<span data-ttu-id="b8091-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8091-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8091-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8091-111">Permission type</span></span>      | <span data-ttu-id="b8091-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8091-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8091-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8091-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b8091-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8091-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b8091-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8091-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8091-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8091-116">Not supported.</span></span>    |
|<span data-ttu-id="b8091-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8091-117">Application</span></span> | <span data-ttu-id="b8091-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8091-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8091-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8091-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="b8091-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8091-120">Request headers</span></span>
| <span data-ttu-id="b8091-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b8091-121">Name</span></span>       | <span data-ttu-id="b8091-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8091-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b8091-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8091-123">Authorization</span></span>  | <span data-ttu-id="b8091-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8091-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8091-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b8091-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="b8091-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b8091-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8091-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8091-129">Request body</span></span>
<span data-ttu-id="b8091-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8091-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b8091-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b8091-131">Parameter</span></span>    | <span data-ttu-id="b8091-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8091-132">Type</span></span>   |<span data-ttu-id="b8091-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8091-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8091-134">address</span><span class="sxs-lookup"><span data-stu-id="b8091-134">address</span></span>|<span data-ttu-id="b8091-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8091-135">string</span></span>|<span data-ttu-id="b8091-p106">Endereço ou nome do objeto de intervalo que representa a fonte de dados. Se o endereço não contiver o nome de uma planilha, a folha ativa no momento será usada.</span><span class="sxs-lookup"><span data-stu-id="b8091-p106">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="b8091-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="b8091-138">hasHeaders</span></span>|<span data-ttu-id="b8091-139">booliano</span><span class="sxs-lookup"><span data-stu-id="b8091-139">boolean</span></span>|<span data-ttu-id="b8091-p107">Valor booliano que indica se os dados que estão sendo importados têm rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="b8091-p107">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="b8091-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8091-143">Response</span></span>

<span data-ttu-id="b8091-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8091-144">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8091-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8091-145">Example</span></span>
<span data-ttu-id="b8091-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b8091-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b8091-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8091-147">Request</span></span>
<span data-ttu-id="b8091-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8091-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b8091-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8091-149">Response</span></span>
<span data-ttu-id="b8091-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8091-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
