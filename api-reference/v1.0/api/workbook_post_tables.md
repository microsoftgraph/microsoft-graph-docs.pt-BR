# <a name="create-table"></a><span data-ttu-id="29635-101">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="29635-101">Create Table</span></span>

<span data-ttu-id="29635-102">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="29635-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="29635-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="29635-103">Permissions</span></span>
<span data-ttu-id="29635-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="29635-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="29635-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29635-106">Permission type</span></span>      | <span data-ttu-id="29635-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29635-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29635-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29635-108">Delegated (work or school account)</span></span> | <span data-ttu-id="29635-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29635-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="29635-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29635-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29635-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29635-111">Not supported.</span></span>    |
|<span data-ttu-id="29635-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29635-112">Application</span></span> | <span data-ttu-id="29635-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29635-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29635-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29635-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="29635-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29635-115">Request headers</span></span>
| <span data-ttu-id="29635-116">Nome</span><span class="sxs-lookup"><span data-stu-id="29635-116">Name</span></span>       | <span data-ttu-id="29635-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="29635-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29635-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="29635-118">Authorization</span></span>  | <span data-ttu-id="29635-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29635-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29635-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29635-121">Request body</span></span>
<span data-ttu-id="29635-122">No corpo da solicitação, forneça uma representação JSON do objeto [Table](../resources/table.md).</span><span class="sxs-lookup"><span data-stu-id="29635-122">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="29635-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="29635-123">Response</span></span>

<span data-ttu-id="29635-124">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29635-124">If successful, this method returns `201, Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29635-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29635-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29635-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29635-126">Request</span></span>
<span data-ttu-id="29635-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29635-127">Here is an example of the request.</span></span>
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
<span data-ttu-id="29635-128">No corpo da solicitação, forneça uma representação JSON do objeto [Table](../resources/table.md).</span><span class="sxs-lookup"><span data-stu-id="29635-128">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="29635-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="29635-129">Response</span></span>
<span data-ttu-id="29635-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29635-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
