# <a name="update-nameditem"></a><span data-ttu-id="49b91-101">Atualizar nameditem</span><span class="sxs-lookup"><span data-stu-id="49b91-101">Update nameditem</span></span>

<span data-ttu-id="49b91-102">Atualize as propriedades do objeto nameditem.</span><span class="sxs-lookup"><span data-stu-id="49b91-102">Update the properties of nameditem object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49b91-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49b91-103">Prerequisites</span></span>
<span data-ttu-id="49b91-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="49b91-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="49b91-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49b91-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="49b91-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49b91-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="49b91-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="49b91-107">Optional request headers</span></span>
| <span data-ttu-id="49b91-108">Nome</span><span class="sxs-lookup"><span data-stu-id="49b91-108">Name</span></span>       | <span data-ttu-id="49b91-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="49b91-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="49b91-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="49b91-110">Authorization</span></span>  | <span data-ttu-id="49b91-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49b91-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="49b91-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49b91-113">Request body</span></span>
<span data-ttu-id="49b91-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="49b91-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="49b91-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49b91-117">Property</span></span>     | <span data-ttu-id="49b91-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="49b91-118">Type</span></span>   |<span data-ttu-id="49b91-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="49b91-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49b91-120">visible</span><span class="sxs-lookup"><span data-stu-id="49b91-120">visible</span></span>|<span data-ttu-id="49b91-121">booliano</span><span class="sxs-lookup"><span data-stu-id="49b91-121">boolean</span></span>|<span data-ttu-id="49b91-122">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="49b91-122">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="49b91-123">comment</span><span class="sxs-lookup"><span data-stu-id="49b91-123">comment</span></span>|   <span data-ttu-id="49b91-124">string</span><span class="sxs-lookup"><span data-stu-id="49b91-124">string</span></span>  |<span data-ttu-id="49b91-125">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="49b91-125">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="49b91-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="49b91-126">Response</span></span>

<span data-ttu-id="49b91-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [NamedItem](../resources/nameditem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49b91-127">If successful, this method returns a `200 OK` response code and updated [NamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49b91-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49b91-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49b91-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49b91-129">Request</span></span>
<span data-ttu-id="49b91-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49b91-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="49b91-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="49b91-131">Response</span></span>
<span data-ttu-id="49b91-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49b91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
