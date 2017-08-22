# <a name="add-named-item-formulalocal"></a><span data-ttu-id="55b42-101">Adicionar item nomeado FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="55b42-101">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="55b42-102">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="55b42-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55b42-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55b42-103">Prerequisites</span></span>
<span data-ttu-id="55b42-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="55b42-104">One of the following **scopes** is required to execute this API:</span></span>

  * <span data-ttu-id="55b42-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55b42-105">Files.ReadWrite</span></span>
  * <span data-ttu-id="55b42-106">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="55b42-106">Sites.Read.All</span></span>
  
## <a name="http-request"></a><span data-ttu-id="55b42-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55b42-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="55b42-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55b42-108">Request headers</span></span>
| <span data-ttu-id="55b42-109">Nome</span><span class="sxs-lookup"><span data-stu-id="55b42-109">Name</span></span>       | <span data-ttu-id="55b42-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="55b42-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="55b42-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="55b42-111">Authorization</span></span>  | <span data-ttu-id="55b42-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55b42-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="55b42-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55b42-114">Request body</span></span>
<span data-ttu-id="55b42-115">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b42-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55b42-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="55b42-116">Parameter</span></span>    | <span data-ttu-id="55b42-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="55b42-117">Type</span></span>   |<span data-ttu-id="55b42-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="55b42-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55b42-119">name</span><span class="sxs-lookup"><span data-stu-id="55b42-119">name</span></span>|<span data-ttu-id="55b42-120">string</span><span class="sxs-lookup"><span data-stu-id="55b42-120">string</span></span>|<span data-ttu-id="55b42-121">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="55b42-121">The name of the named item.</span></span>|
|<span data-ttu-id="55b42-122">formula</span><span class="sxs-lookup"><span data-stu-id="55b42-122">formula</span></span>|<span data-ttu-id="55b42-123">string</span><span class="sxs-lookup"><span data-stu-id="55b42-123">string</span></span>|<span data-ttu-id="55b42-124">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="55b42-124">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="55b42-125">comentário</span><span class="sxs-lookup"><span data-stu-id="55b42-125">comment</span></span>|<span data-ttu-id="55b42-126">string</span><span class="sxs-lookup"><span data-stu-id="55b42-126">string</span></span>|<span data-ttu-id="55b42-127">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="55b42-127">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="55b42-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b42-128">Response</span></span>

<span data-ttu-id="55b42-129">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [NamedItem](../resources/NamedItem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55b42-129">If successful, this method returns `200, OK` response code and [NamedItem](../resources/NamedItem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55b42-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55b42-130">Example</span></span>
<span data-ttu-id="55b42-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="55b42-131">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="55b42-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55b42-132">Request</span></span>
<span data-ttu-id="55b42-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b42-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a><span data-ttu-id="55b42-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b42-134">Response</span></span>
<span data-ttu-id="55b42-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55b42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "Double",
    "value": 0,
    "visible": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
