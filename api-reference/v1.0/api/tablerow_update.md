# <a name="update-tablerow"></a><span data-ttu-id="e8bfa-101">Atualizar tablerow</span><span class="sxs-lookup"><span data-stu-id="e8bfa-101">Update tablerow</span></span>

<span data-ttu-id="e8bfa-102">Atualize as propriedades do objeto tablerow.</span><span class="sxs-lookup"><span data-stu-id="e8bfa-102">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8bfa-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8bfa-103">Permissions</span></span>
<span data-ttu-id="e8bfa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8bfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8bfa-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8bfa-106">Permission type</span></span>      | <span data-ttu-id="e8bfa-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8bfa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8bfa-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8bfa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e8bfa-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8bfa-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8bfa-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8bfa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8bfa-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8bfa-111">Not supported.</span></span>    |
|<span data-ttu-id="e8bfa-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8bfa-112">Application</span></span> | <span data-ttu-id="e8bfa-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8bfa-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8bfa-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8bfa-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows(<index>)
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="e8bfa-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e8bfa-115">Optional request headers</span></span>
| <span data-ttu-id="e8bfa-116">Nome</span><span class="sxs-lookup"><span data-stu-id="e8bfa-116">Name</span></span>       | <span data-ttu-id="e8bfa-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8bfa-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e8bfa-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8bfa-118">Authorization</span></span>  | <span data-ttu-id="e8bfa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8bfa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8bfa-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8bfa-121">Request body</span></span>
<span data-ttu-id="e8bfa-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e8bfa-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e8bfa-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8bfa-125">Property</span></span>     | <span data-ttu-id="e8bfa-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8bfa-126">Type</span></span>   |<span data-ttu-id="e8bfa-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8bfa-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8bfa-128">values</span><span class="sxs-lookup"><span data-stu-id="e8bfa-128">values</span></span>|<span data-ttu-id="e8bfa-129">json</span><span class="sxs-lookup"><span data-stu-id="e8bfa-129">json</span></span>|<span data-ttu-id="e8bfa-p104">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="e8bfa-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="e8bfa-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8bfa-133">Response</span></span>

<span data-ttu-id="e8bfa-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TableRow](../resources/tablerow.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8bfa-134">If successful, this method returns a `200 OK` response code and updated [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8bfa-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8bfa-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8bfa-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8bfa-136">Request</span></span>
<span data-ttu-id="e8bfa-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8bfa-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="e8bfa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8bfa-138">Response</span></span>
<span data-ttu-id="e8bfa-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8bfa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->