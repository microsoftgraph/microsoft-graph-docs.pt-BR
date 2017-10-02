# <a name="add-named-item-formulalocal"></a><span data-ttu-id="f7d9c-101">Adicionar item nomeado FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="f7d9c-101">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="f7d9c-102">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7d9c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7d9c-103">Permissions</span></span>
<span data-ttu-id="f7d9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7d9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f7d9c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7d9c-106">Permission type</span></span>      | <span data-ttu-id="f7d9c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7d9c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7d9c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7d9c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f7d9c-109">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7d9c-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="f7d9c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7d9c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7d9c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-111">Not supported.</span></span>    |
|<span data-ttu-id="f7d9c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7d9c-112">Application</span></span> | <span data-ttu-id="f7d9c-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7d9c-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7d9c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7d9c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="f7d9c-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d9c-115">Request headers</span></span>
| <span data-ttu-id="f7d9c-116">Nome</span><span class="sxs-lookup"><span data-stu-id="f7d9c-116">Name</span></span>       | <span data-ttu-id="f7d9c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7d9c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7d9c-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7d9c-118">Authorization</span></span>  | <span data-ttu-id="f7d9c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7d9c-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d9c-121">Request body</span></span>
<span data-ttu-id="f7d9c-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7d9c-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f7d9c-123">Parameter</span></span>    | <span data-ttu-id="f7d9c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7d9c-124">Type</span></span>   |<span data-ttu-id="f7d9c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7d9c-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7d9c-126">name</span><span class="sxs-lookup"><span data-stu-id="f7d9c-126">name</span></span>|<span data-ttu-id="f7d9c-127">string</span><span class="sxs-lookup"><span data-stu-id="f7d9c-127">string</span></span>|<span data-ttu-id="f7d9c-128">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-128">The name of the named item.</span></span>|
|<span data-ttu-id="f7d9c-129">formula</span><span class="sxs-lookup"><span data-stu-id="f7d9c-129">formula</span></span>|<span data-ttu-id="f7d9c-130">string</span><span class="sxs-lookup"><span data-stu-id="f7d9c-130">string</span></span>|<span data-ttu-id="f7d9c-131">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-131">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="f7d9c-132">comentário</span><span class="sxs-lookup"><span data-stu-id="f7d9c-132">comment</span></span>|<span data-ttu-id="f7d9c-133">string</span><span class="sxs-lookup"><span data-stu-id="f7d9c-133">string</span></span>|<span data-ttu-id="f7d9c-134">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="f7d9c-134">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="f7d9c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7d9c-135">Response</span></span>

<span data-ttu-id="f7d9c-136">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [NamedItem](../resources/NamedItem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-136">If successful, this method returns `200, OK` response code and [NamedItem](../resources/NamedItem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7d9c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7d9c-137">Example</span></span>
<span data-ttu-id="f7d9c-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f7d9c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d9c-139">Request</span></span>
<span data-ttu-id="f7d9c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-140">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="f7d9c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7d9c-141">Response</span></span>
<span data-ttu-id="f7d9c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7d9c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "value": "0",
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
