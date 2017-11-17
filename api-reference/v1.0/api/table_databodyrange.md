# <a name="table-databodyrange"></a><span data-ttu-id="5e9cf-101">Table: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="5e9cf-101">Table: DataBodyRange</span></span>

<span data-ttu-id="5e9cf-102">Obtém o objeto de intervalo associado ao corpo de dados da tabela.</span><span class="sxs-lookup"><span data-stu-id="5e9cf-102">Gets the range object associated with the data body of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e9cf-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e9cf-103">Permissions</span></span>
<span data-ttu-id="5e9cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e9cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5e9cf-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e9cf-106">Permission type</span></span>      | <span data-ttu-id="5e9cf-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e9cf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e9cf-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e9cf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5e9cf-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e9cf-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e9cf-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e9cf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e9cf-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e9cf-111">Not supported.</span></span>    |
|<span data-ttu-id="5e9cf-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e9cf-112">Application</span></span> | <span data-ttu-id="5e9cf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e9cf-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e9cf-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e9cf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/DataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/DataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="5e9cf-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e9cf-115">Request headers</span></span>
| <span data-ttu-id="5e9cf-116">Nome</span><span class="sxs-lookup"><span data-stu-id="5e9cf-116">Name</span></span>       | <span data-ttu-id="5e9cf-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e9cf-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5e9cf-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e9cf-118">Authorization</span></span>  | <span data-ttu-id="5e9cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e9cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e9cf-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e9cf-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5e9cf-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e9cf-122">Response</span></span>

<span data-ttu-id="5e9cf-123">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e9cf-123">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e9cf-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e9cf-124">Example</span></span>
<span data-ttu-id="5e9cf-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5e9cf-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5e9cf-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e9cf-126">Request</span></span>
<span data-ttu-id="5e9cf-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e9cf-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_databodyrange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/DataBodyRange
```

##### <a name="response"></a><span data-ttu-id="5e9cf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e9cf-128">Response</span></span>
<span data-ttu-id="5e9cf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e9cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->