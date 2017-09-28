# <a name="chartfill-clear"></a><span data-ttu-id="f7d78-101">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="f7d78-101">ChartFill: clear</span></span>

<span data-ttu-id="f7d78-102">Limpe a cor de preenchimento de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="f7d78-102">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7d78-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="f7d78-103">Permissions</span></span>
<span data-ttu-id="f7d78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7d78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f7d78-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7d78-106">Permission type</span></span>      | <span data-ttu-id="f7d78-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7d78-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7d78-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7d78-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f7d78-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7d78-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7d78-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7d78-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7d78-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7d78-111">Not supported.</span></span>    |
|<span data-ttu-id="f7d78-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7d78-112">Application</span></span> | <span data-ttu-id="f7d78-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7d78-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7d78-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7d78-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="f7d78-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d78-115">Request headers</span></span>
| <span data-ttu-id="f7d78-116">Nome</span><span class="sxs-lookup"><span data-stu-id="f7d78-116">Name</span></span>       | <span data-ttu-id="f7d78-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7d78-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7d78-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7d78-118">Authorization</span></span>  | <span data-ttu-id="f7d78-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7d78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7d78-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d78-121">Request body</span></span>
<span data-ttu-id="f7d78-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7d78-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7d78-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7d78-123">Response</span></span>

<span data-ttu-id="f7d78-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7d78-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7d78-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7d78-126">Example</span></span>
<span data-ttu-id="f7d78-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f7d78-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7d78-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d78-128">Request</span></span>
<span data-ttu-id="f7d78-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7d78-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="f7d78-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7d78-130">Response</span></span>
<span data-ttu-id="f7d78-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7d78-131">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->