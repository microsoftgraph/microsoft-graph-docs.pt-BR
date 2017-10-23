# <a name="range-clear"></a><span data-ttu-id="c229e-101">Range: clear</span><span class="sxs-lookup"><span data-stu-id="c229e-101">Range: clear</span></span>

<span data-ttu-id="c229e-102">Limpa valores de intervalo, formatação, preenchimento, borda, etc.</span><span class="sxs-lookup"><span data-stu-id="c229e-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="c229e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="c229e-103">Permissions</span></span>
<span data-ttu-id="c229e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c229e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c229e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c229e-106">Permission type</span></span>      | <span data-ttu-id="c229e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c229e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c229e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c229e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c229e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c229e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c229e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c229e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c229e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c229e-111">Not supported.</span></span>    |
|<span data-ttu-id="c229e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c229e-112">Application</span></span> | <span data-ttu-id="c229e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c229e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c229e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c229e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/clear
GET /workbook/worksheets/{id|name}/range(<address>)/clear
GET /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="c229e-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c229e-115">Request headers</span></span>
| <span data-ttu-id="c229e-116">Nome</span><span class="sxs-lookup"><span data-stu-id="c229e-116">Name</span></span>       | <span data-ttu-id="c229e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c229e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c229e-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="c229e-118">Authorization</span></span>  | <span data-ttu-id="c229e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c229e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c229e-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c229e-121">Request body</span></span>
<span data-ttu-id="c229e-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c229e-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c229e-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c229e-123">Parameter</span></span>    | <span data-ttu-id="c229e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c229e-124">Type</span></span>   |<span data-ttu-id="c229e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c229e-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c229e-126">applyTo</span><span class="sxs-lookup"><span data-stu-id="c229e-126">applyTo</span></span>|<span data-ttu-id="c229e-127">string</span><span class="sxs-lookup"><span data-stu-id="c229e-127">string</span></span>|<span data-ttu-id="c229e-p103">Opcional. Determina o tipo de ação de limpeza.  Os valores possíveis são: `All`, `Formats` e `Contents`.</span><span class="sxs-lookup"><span data-stu-id="c229e-p103">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="c229e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c229e-131">Response</span></span>

<span data-ttu-id="c229e-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c229e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c229e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c229e-134">Example</span></span>
<span data-ttu-id="c229e-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c229e-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c229e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c229e-136">Request</span></span>
<span data-ttu-id="c229e-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c229e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="c229e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c229e-138">Response</span></span>
<span data-ttu-id="c229e-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c229e-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->