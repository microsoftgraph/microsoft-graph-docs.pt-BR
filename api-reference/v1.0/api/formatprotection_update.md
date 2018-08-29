# <a name="update-formatprotection"></a><span data-ttu-id="e1a48-101">Atualizar formatprotection</span><span class="sxs-lookup"><span data-stu-id="e1a48-101">Update formatprotection</span></span>

<span data-ttu-id="e1a48-102">Atualiza as propriedades do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="e1a48-102">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1a48-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1a48-103">Permissions</span></span>
<span data-ttu-id="e1a48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1a48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1a48-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1a48-106">Permission type</span></span>      | <span data-ttu-id="e1a48-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1a48-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e1a48-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1a48-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e1a48-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a48-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="e1a48-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1a48-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1a48-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1a48-111">Not supported.</span></span>    | 
|<span data-ttu-id="e1a48-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1a48-112">Application</span></span> | <span data-ttu-id="e1a48-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1a48-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e1a48-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1a48-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="e1a48-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e1a48-115">Optional request headers</span></span>
| <span data-ttu-id="e1a48-116">Nome</span><span class="sxs-lookup"><span data-stu-id="e1a48-116">Name</span></span>       | <span data-ttu-id="e1a48-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1a48-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e1a48-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1a48-118">Authorization</span></span>  | <span data-ttu-id="e1a48-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1a48-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e1a48-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1a48-121">Request body</span></span>
<span data-ttu-id="e1a48-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e1a48-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e1a48-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1a48-125">Property</span></span>     | <span data-ttu-id="e1a48-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1a48-126">Type</span></span>   |<span data-ttu-id="e1a48-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1a48-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1a48-128">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="e1a48-128">formulaHidden</span></span>|<span data-ttu-id="e1a48-129">booliano</span><span class="sxs-lookup"><span data-stu-id="e1a48-129">boolean</span></span>|<span data-ttu-id="e1a48-p104">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="e1a48-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="e1a48-132">locked</span><span class="sxs-lookup"><span data-stu-id="e1a48-132">locked</span></span>|<span data-ttu-id="e1a48-133">booliano</span><span class="sxs-lookup"><span data-stu-id="e1a48-133">boolean</span></span>|<span data-ttu-id="e1a48-p105">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="e1a48-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="e1a48-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1a48-136">Response</span></span>

<span data-ttu-id="e1a48-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1a48-137">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e1a48-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1a48-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1a48-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1a48-139">Request</span></span>
<span data-ttu-id="e1a48-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1a48-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="e1a48-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1a48-141">Response</span></span>
<span data-ttu-id="e1a48-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1a48-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
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