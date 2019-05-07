---
title: Adicionar item nomeado FormulaLocal
description: Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.
localization_priority: Normal
ms.openlocfilehash: 452707d546e7f0b358a840056b03271ca1a0c7ee
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612122"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="56ffc-103">Adicionar item nomeado FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="56ffc-103">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="56ffc-104">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="56ffc-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="56ffc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="56ffc-105">Permissions</span></span>
<span data-ttu-id="56ffc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56ffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56ffc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56ffc-108">Permission type</span></span>      | <span data-ttu-id="56ffc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56ffc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56ffc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56ffc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56ffc-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="56ffc-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="56ffc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56ffc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56ffc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56ffc-113">Not supported.</span></span>    |
|<span data-ttu-id="56ffc-114">Application</span><span class="sxs-lookup"><span data-stu-id="56ffc-114">Application</span></span> | <span data-ttu-id="56ffc-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="56ffc-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56ffc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56ffc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="56ffc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56ffc-117">Request headers</span></span>
| <span data-ttu-id="56ffc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="56ffc-118">Name</span></span>       | <span data-ttu-id="56ffc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ffc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56ffc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="56ffc-120">Authorization</span></span>  | <span data-ttu-id="56ffc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56ffc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56ffc-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="56ffc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="56ffc-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="56ffc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56ffc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56ffc-126">Request body</span></span>
<span data-ttu-id="56ffc-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56ffc-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56ffc-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="56ffc-128">Parameter</span></span>    | <span data-ttu-id="56ffc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="56ffc-129">Type</span></span>   |<span data-ttu-id="56ffc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ffc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56ffc-131">nome</span><span class="sxs-lookup"><span data-stu-id="56ffc-131">name</span></span>|<span data-ttu-id="56ffc-132">string</span><span class="sxs-lookup"><span data-stu-id="56ffc-132">string</span></span>|<span data-ttu-id="56ffc-133">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="56ffc-133">The name of the named item.</span></span>|
|<span data-ttu-id="56ffc-134">formula</span><span class="sxs-lookup"><span data-stu-id="56ffc-134">formula</span></span>|<span data-ttu-id="56ffc-135">string</span><span class="sxs-lookup"><span data-stu-id="56ffc-135">string</span></span>|<span data-ttu-id="56ffc-136">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="56ffc-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="56ffc-137">comentário</span><span class="sxs-lookup"><span data-stu-id="56ffc-137">comment</span></span>|<span data-ttu-id="56ffc-138">string</span><span class="sxs-lookup"><span data-stu-id="56ffc-138">string</span></span>|<span data-ttu-id="56ffc-139">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="56ffc-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="56ffc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ffc-140">Response</span></span>

<span data-ttu-id="56ffc-141">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookNamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56ffc-141">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56ffc-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56ffc-142">Example</span></span>
<span data-ttu-id="56ffc-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="56ffc-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="56ffc-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56ffc-144">Request</span></span>
<span data-ttu-id="56ffc-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56ffc-145">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="56ffc-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ffc-146">Response</span></span>
<span data-ttu-id="56ffc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56ffc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="56ffc-150">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="56ffc-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="56ffc-151">Basic</span><span class="sxs-lookup"><span data-stu-id="56ffc-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/NamedItemcollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56ffc-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56ffc-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/NamedItemcollection_add-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/nameditem-addformulalocal.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/nameditem-addformulalocal.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
