# <a name="create-table"></a><span data-ttu-id="a18aa-101">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="a18aa-101">Create Table</span></span>

<span data-ttu-id="a18aa-102">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="a18aa-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="a18aa-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a18aa-103">Permissions</span></span>
<span data-ttu-id="a18aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a18aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a18aa-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a18aa-106">Permission type</span></span>      | <span data-ttu-id="a18aa-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a18aa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a18aa-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a18aa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a18aa-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a18aa-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a18aa-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a18aa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a18aa-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a18aa-111">Not supported.</span></span>    |
|<span data-ttu-id="a18aa-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a18aa-112">Application</span></span> | <span data-ttu-id="a18aa-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a18aa-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a18aa-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a18aa-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{table-id}/add

```
## <a name="request-headers"></a><span data-ttu-id="a18aa-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a18aa-115">Request headers</span></span>
| <span data-ttu-id="a18aa-116">Nome</span><span class="sxs-lookup"><span data-stu-id="a18aa-116">Name</span></span>       | <span data-ttu-id="a18aa-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a18aa-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a18aa-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="a18aa-118">Authorization</span></span>  | <span data-ttu-id="a18aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a18aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a18aa-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a18aa-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a18aa-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a18aa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

### <a name="request-parameters"></a><span data-ttu-id="a18aa-124">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="a18aa-124">Request parameters</span></span>
| <span data-ttu-id="a18aa-125">Nome</span><span class="sxs-lookup"><span data-stu-id="a18aa-125">Name</span></span>           | <span data-ttu-id="a18aa-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a18aa-126">Type</span></span>      |<span data-ttu-id="a18aa-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a18aa-127">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="a18aa-128">Endereço</span><span class="sxs-lookup"><span data-stu-id="a18aa-128">Address</span></span>  | <span data-ttu-id="a18aa-129">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a18aa-129">string</span></span>| <span data-ttu-id="a18aa-p104">Endereço do intervalo. Se você estiver chamando essa API fora do caminho `worksheets/{id or name}/tables/add`, não haverá necessidade do prefixo de nome da planilha no endereço. No entanto, se você a estiver chamando fora do caminho `workbook/tables/add`, forneça então o nome da planilha em que a tabela precisa ser criada (exemplo: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="a18aa-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="a18aa-133">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="a18aa-133">hasHeaders</span></span>  | <span data-ttu-id="a18aa-134">booliano</span><span class="sxs-lookup"><span data-stu-id="a18aa-134">boolean</span></span>|<span data-ttu-id="a18aa-p105">O valor booliano que indica se o intervalo tem rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="a18aa-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="a18aa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a18aa-138">Response</span></span>

<span data-ttu-id="a18aa-139">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [WorkbookTable](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a18aa-139">If successful, this method returns `201 Created` response code and [groupSetting](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a18aa-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a18aa-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a18aa-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a18aa-141">Request</span></span>
<span data-ttu-id="a18aa-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a18aa-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{table-id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="a18aa-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a18aa-143">Response</span></span>
<span data-ttu-id="a18aa-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a18aa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
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
