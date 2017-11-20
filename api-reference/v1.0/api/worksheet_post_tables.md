# <a name="create-table"></a><span data-ttu-id="fcabd-101">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="fcabd-101">Create Table</span></span>

<span data-ttu-id="fcabd-102">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="fcabd-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="fcabd-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="fcabd-103">Permissions</span></span>
<span data-ttu-id="fcabd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcabd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fcabd-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcabd-106">Permission type</span></span>      | <span data-ttu-id="fcabd-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcabd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcabd-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcabd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fcabd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcabd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fcabd-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcabd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcabd-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcabd-111">Not supported.</span></span>    |
|<span data-ttu-id="fcabd-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcabd-112">Application</span></span> | <span data-ttu-id="fcabd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcabd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcabd-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcabd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="fcabd-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcabd-115">Request headers</span></span>
| <span data-ttu-id="fcabd-116">Nome</span><span class="sxs-lookup"><span data-stu-id="fcabd-116">Name</span></span>       | <span data-ttu-id="fcabd-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcabd-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fcabd-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcabd-118">Authorization</span></span>  | <span data-ttu-id="fcabd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcabd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fcabd-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fcabd-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="fcabd-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fcabd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcabd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcabd-124">Request body</span></span>
<span data-ttu-id="fcabd-125">No corpo da solicitação, forneça os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fcabd-125">In the request body, supply following parameters.</span></span> 

### <a name="request-parameters"></a><span data-ttu-id="fcabd-126">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="fcabd-126">Request parameters</span></span>
| <span data-ttu-id="fcabd-127">Nome</span><span class="sxs-lookup"><span data-stu-id="fcabd-127">Name</span></span>           | <span data-ttu-id="fcabd-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcabd-128">Type</span></span>      |<span data-ttu-id="fcabd-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcabd-129">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="fcabd-130">Endereço</span><span class="sxs-lookup"><span data-stu-id="fcabd-130">Address</span></span>  | <span data-ttu-id="fcabd-131">string</span><span class="sxs-lookup"><span data-stu-id="fcabd-131">string</span></span>| <span data-ttu-id="fcabd-p104">Endereço do intervalo. Se você estiver chamando essa API fora do caminho `worksheets/{id or name}/tables/add`, não haverá necessidade do prefixo de nome da planilha no endereço. No entanto, se você a estiver chamando fora do caminho `workbook/tables/add`, forneça então o nome da planilha em que a tabela precisa ser criada (exemplo: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="fcabd-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="fcabd-135">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="fcabd-135">hasHeaders</span></span>  | <span data-ttu-id="fcabd-136">booliano</span><span class="sxs-lookup"><span data-stu-id="fcabd-136">boolean</span></span>|<span data-ttu-id="fcabd-p105">O valor booliano que indica se o intervalo tem rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="fcabd-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="fcabd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcabd-140">Response</span></span>

<span data-ttu-id="fcabd-141">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcabd-141">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcabd-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcabd-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcabd-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcabd-143">Request</span></span>
<span data-ttu-id="fcabd-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcabd-144">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fcabd-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcabd-145">Response</span></span>
<span data-ttu-id="fcabd-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcabd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
