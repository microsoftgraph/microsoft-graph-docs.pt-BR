# <a name="create-chartpoints"></a><span data-ttu-id="98007-101">Criar ChartPoints</span><span class="sxs-lookup"><span data-stu-id="98007-101">Create ChartPoints</span></span>

<span data-ttu-id="98007-102">Use essa API para criar novos ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="98007-102">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="98007-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="98007-103">Permissions</span></span>
<span data-ttu-id="98007-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="98007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="98007-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98007-106">Permission type</span></span>      | <span data-ttu-id="98007-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98007-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98007-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98007-108">Delegated (work or school account)</span></span> | <span data-ttu-id="98007-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98007-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="98007-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98007-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98007-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98007-111">Not supported.</span></span>    |
|<span data-ttu-id="98007-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98007-112">Application</span></span> | <span data-ttu-id="98007-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98007-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98007-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98007-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="98007-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98007-115">Request headers</span></span>
| <span data-ttu-id="98007-116">Nome</span><span class="sxs-lookup"><span data-stu-id="98007-116">Name</span></span>       | <span data-ttu-id="98007-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="98007-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98007-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="98007-118">Authorization</span></span>  | <span data-ttu-id="98007-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98007-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98007-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98007-121">Request body</span></span>
<span data-ttu-id="98007-122">No corpo da solicitação, forneça uma representação JSON do objeto [ChartPoints](../resources/chartpoint.md).</span><span class="sxs-lookup"><span data-stu-id="98007-122">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="98007-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="98007-123">Response</span></span>

<span data-ttu-id="98007-124">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ChartPoints](../resources/chartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98007-124">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98007-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98007-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98007-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98007-126">Request</span></span>
<span data-ttu-id="98007-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98007-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="98007-128">No corpo da solicitação, forneça uma representação JSON do objeto [ChartPoints](../resources/chartpoint.md).</span><span class="sxs-lookup"><span data-stu-id="98007-128">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="98007-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="98007-129">Response</span></span>
<span data-ttu-id="98007-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98007-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->