# <a name="update-formatprotection"></a><span data-ttu-id="b95f3-101">Atualizar formatprotection</span><span class="sxs-lookup"><span data-stu-id="b95f3-101">Update formatprotection</span></span>

<span data-ttu-id="b95f3-102">Atualiza as propriedades do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="b95f3-102">Update the properties of formatprotection object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b95f3-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b95f3-103">Prerequisites</span></span>
<span data-ttu-id="b95f3-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="b95f3-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="b95f3-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b95f3-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="b95f3-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b95f3-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="b95f3-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b95f3-107">Optional request headers</span></span>
| <span data-ttu-id="b95f3-108">Nome</span><span class="sxs-lookup"><span data-stu-id="b95f3-108">Name</span></span>       | <span data-ttu-id="b95f3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b95f3-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b95f3-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="b95f3-110">Authorization</span></span>  | <span data-ttu-id="b95f3-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b95f3-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b95f3-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b95f3-113">Request body</span></span>
<span data-ttu-id="b95f3-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b95f3-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b95f3-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b95f3-117">Property</span></span>     | <span data-ttu-id="b95f3-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="b95f3-118">Type</span></span>   |<span data-ttu-id="b95f3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b95f3-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b95f3-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="b95f3-120">formulaHidden</span></span>|<span data-ttu-id="b95f3-121">booliano</span><span class="sxs-lookup"><span data-stu-id="b95f3-121">boolean</span></span>|<span data-ttu-id="b95f3-p103">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="b95f3-p103">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="b95f3-124">locked</span><span class="sxs-lookup"><span data-stu-id="b95f3-124">locked</span></span>|<span data-ttu-id="b95f3-125">booliano</span><span class="sxs-lookup"><span data-stu-id="b95f3-125">boolean</span></span>|<span data-ttu-id="b95f3-p104">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="b95f3-p104">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="b95f3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95f3-128">Response</span></span>

<span data-ttu-id="b95f3-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b95f3-129">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b95f3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b95f3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b95f3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b95f3-131">Request</span></span>
<span data-ttu-id="b95f3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b95f3-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="b95f3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95f3-133">Response</span></span>
<span data-ttu-id="b95f3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b95f3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->