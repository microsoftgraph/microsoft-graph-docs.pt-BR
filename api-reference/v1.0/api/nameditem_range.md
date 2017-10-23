# <a name="nameditem-range"></a><span data-ttu-id="72a0e-101">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="72a0e-101">NamedItem: Range</span></span>

<span data-ttu-id="72a0e-p101">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="72a0e-p101">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="72a0e-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="72a0e-104">Permissions</span></span>
<span data-ttu-id="72a0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="72a0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="72a0e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72a0e-107">Permission type</span></span>      | <span data-ttu-id="72a0e-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72a0e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72a0e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72a0e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="72a0e-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72a0e-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="72a0e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72a0e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72a0e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72a0e-112">Not supported.</span></span>    |
|<span data-ttu-id="72a0e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72a0e-113">Application</span></span> | <span data-ttu-id="72a0e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72a0e-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72a0e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72a0e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/Range

```
## <a name="request-headers"></a><span data-ttu-id="72a0e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72a0e-116">Request headers</span></span>
| <span data-ttu-id="72a0e-117">Nome</span><span class="sxs-lookup"><span data-stu-id="72a0e-117">Name</span></span>       | <span data-ttu-id="72a0e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="72a0e-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72a0e-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="72a0e-119">Authorization</span></span>  | <span data-ttu-id="72a0e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72a0e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72a0e-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72a0e-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="72a0e-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="72a0e-123">Response</span></span>

<span data-ttu-id="72a0e-124">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72a0e-124">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72a0e-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72a0e-125">Example</span></span>
<span data-ttu-id="72a0e-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="72a0e-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="72a0e-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72a0e-127">Request</span></span>
<span data-ttu-id="72a0e-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72a0e-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/Range
```

##### <a name="response"></a><span data-ttu-id="72a0e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="72a0e-129">Response</span></span>
<span data-ttu-id="72a0e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72a0e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->