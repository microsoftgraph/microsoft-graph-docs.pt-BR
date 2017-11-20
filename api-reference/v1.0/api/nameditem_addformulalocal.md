# <a name="add-named-item-formulalocal"></a><span data-ttu-id="06ed9-101">Adicionar item nomeado FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="06ed9-101">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="06ed9-102">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="06ed9-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="06ed9-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="06ed9-103">Permissions</span></span>
<span data-ttu-id="06ed9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="06ed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06ed9-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06ed9-106">Permission type</span></span>      | <span data-ttu-id="06ed9-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06ed9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06ed9-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06ed9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="06ed9-109">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="06ed9-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="06ed9-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06ed9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06ed9-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06ed9-111">Not supported.</span></span>    |
|<span data-ttu-id="06ed9-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06ed9-112">Application</span></span> | <span data-ttu-id="06ed9-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="06ed9-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06ed9-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06ed9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="06ed9-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06ed9-115">Request headers</span></span>
| <span data-ttu-id="06ed9-116">Nome</span><span class="sxs-lookup"><span data-stu-id="06ed9-116">Name</span></span>       | <span data-ttu-id="06ed9-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="06ed9-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="06ed9-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="06ed9-118">Authorization</span></span>  | <span data-ttu-id="06ed9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06ed9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06ed9-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="06ed9-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="06ed9-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="06ed9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06ed9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06ed9-124">Request body</span></span>
<span data-ttu-id="06ed9-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06ed9-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="06ed9-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="06ed9-126">Parameter</span></span>    | <span data-ttu-id="06ed9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="06ed9-127">Type</span></span>   |<span data-ttu-id="06ed9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="06ed9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06ed9-129">name</span><span class="sxs-lookup"><span data-stu-id="06ed9-129">name</span></span>|<span data-ttu-id="06ed9-130">string</span><span class="sxs-lookup"><span data-stu-id="06ed9-130">string</span></span>|<span data-ttu-id="06ed9-131">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="06ed9-131">The name of the named item.</span></span>|
|<span data-ttu-id="06ed9-132">formula</span><span class="sxs-lookup"><span data-stu-id="06ed9-132">formula</span></span>|<span data-ttu-id="06ed9-133">string</span><span class="sxs-lookup"><span data-stu-id="06ed9-133">string</span></span>|<span data-ttu-id="06ed9-134">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="06ed9-134">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="06ed9-135">comentário</span><span class="sxs-lookup"><span data-stu-id="06ed9-135">comment</span></span>|<span data-ttu-id="06ed9-136">string</span><span class="sxs-lookup"><span data-stu-id="06ed9-136">string</span></span>|<span data-ttu-id="06ed9-137">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="06ed9-137">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="06ed9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="06ed9-138">Response</span></span>

<span data-ttu-id="06ed9-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [NamedItem](../resources/NamedItem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06ed9-139">If successful, this method returns `200 OK` response code and [NamedItem](../resources/NamedItem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06ed9-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06ed9-140">Example</span></span>
<span data-ttu-id="06ed9-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="06ed9-141">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="06ed9-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06ed9-142">Request</span></span>
<span data-ttu-id="06ed9-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06ed9-143">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="06ed9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="06ed9-144">Response</span></span>
<span data-ttu-id="06ed9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06ed9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "type": "String",
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
