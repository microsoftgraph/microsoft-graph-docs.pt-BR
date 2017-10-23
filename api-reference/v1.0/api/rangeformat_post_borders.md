# <a name="create-rangeborder"></a><span data-ttu-id="83a0c-101">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="83a0c-101">Create RangeBorder</span></span>

<span data-ttu-id="83a0c-102">Use essa API para criar uma nova RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="83a0c-102">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="83a0c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="83a0c-103">Permissions</span></span>
<span data-ttu-id="83a0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="83a0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="83a0c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83a0c-106">Permission type</span></span>      | <span data-ttu-id="83a0c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83a0c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83a0c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83a0c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="83a0c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83a0c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="83a0c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83a0c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83a0c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83a0c-111">Not supported.</span></span>    |
|<span data-ttu-id="83a0c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83a0c-112">Application</span></span> | <span data-ttu-id="83a0c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83a0c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83a0c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83a0c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(<address>)/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="83a0c-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83a0c-115">Request headers</span></span>
| <span data-ttu-id="83a0c-116">Nome</span><span class="sxs-lookup"><span data-stu-id="83a0c-116">Name</span></span>       | <span data-ttu-id="83a0c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="83a0c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="83a0c-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="83a0c-118">Authorization</span></span>  | <span data-ttu-id="83a0c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83a0c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83a0c-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83a0c-121">Request body</span></span>
<span data-ttu-id="83a0c-122">No corpo da solicitação, forneça uma representação JSON do objeto [RangeBorder](../resources/rangeborder.md).</span><span class="sxs-lookup"><span data-stu-id="83a0c-122">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="83a0c-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a0c-123">Response</span></span>

<span data-ttu-id="83a0c-124">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [RangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83a0c-124">If successful, this method returns `201 Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83a0c-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83a0c-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83a0c-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83a0c-126">Request</span></span>
<span data-ttu-id="83a0c-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83a0c-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="83a0c-128">No corpo da solicitação, forneça uma representação JSON do objeto [RangeBorder](../resources/rangeborder.md).</span><span class="sxs-lookup"><span data-stu-id="83a0c-128">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="83a0c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a0c-129">Response</span></span>
<span data-ttu-id="83a0c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83a0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->