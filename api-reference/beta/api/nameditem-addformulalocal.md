---
title: Adicionar item nomeado FormulaLocal
description: Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f712700a2421eec2149b4b8ebc7aa0c610ecf781
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414872"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="099c7-103">Adicionar item nomeado FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="099c7-103">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="099c7-104">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="099c7-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="099c7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="099c7-105">Permissions</span></span>
<span data-ttu-id="099c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="099c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="099c7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="099c7-108">Permission type</span></span>      | <span data-ttu-id="099c7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="099c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="099c7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="099c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="099c7-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="099c7-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="099c7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="099c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="099c7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="099c7-113">Not supported.</span></span>    |
|<span data-ttu-id="099c7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="099c7-114">Application</span></span> | <span data-ttu-id="099c7-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="099c7-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="099c7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="099c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="099c7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="099c7-117">Request headers</span></span>
| <span data-ttu-id="099c7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="099c7-118">Name</span></span>       | <span data-ttu-id="099c7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="099c7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="099c7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="099c7-120">Authorization</span></span>  | <span data-ttu-id="099c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="099c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="099c7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="099c7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="099c7-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="099c7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="099c7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="099c7-126">Request body</span></span>
<span data-ttu-id="099c7-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="099c7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="099c7-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="099c7-128">Parameter</span></span>    | <span data-ttu-id="099c7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="099c7-129">Type</span></span>   |<span data-ttu-id="099c7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="099c7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="099c7-131">name</span><span class="sxs-lookup"><span data-stu-id="099c7-131">name</span></span>|<span data-ttu-id="099c7-132">string</span><span class="sxs-lookup"><span data-stu-id="099c7-132">string</span></span>|<span data-ttu-id="099c7-133">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="099c7-133">The name of the named item.</span></span>|
|<span data-ttu-id="099c7-134">formula</span><span class="sxs-lookup"><span data-stu-id="099c7-134">formula</span></span>|<span data-ttu-id="099c7-135">string</span><span class="sxs-lookup"><span data-stu-id="099c7-135">string</span></span>|<span data-ttu-id="099c7-136">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="099c7-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="099c7-137">comentário</span><span class="sxs-lookup"><span data-stu-id="099c7-137">comment</span></span>|<span data-ttu-id="099c7-138">string</span><span class="sxs-lookup"><span data-stu-id="099c7-138">string</span></span>|<span data-ttu-id="099c7-139">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="099c7-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="099c7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="099c7-140">Response</span></span>

<span data-ttu-id="099c7-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [NamedItem](../resources/workbooknameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="099c7-141">If successful, this method returns `200 OK` response code and [NamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="099c7-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="099c7-142">Example</span></span>
<span data-ttu-id="099c7-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="099c7-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="099c7-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="099c7-144">Request</span></span>
<span data-ttu-id="099c7-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="099c7-145">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="099c7-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="099c7-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="099c7-147">C#</span><span class="sxs-lookup"><span data-stu-id="099c7-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="099c7-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="099c7-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="099c7-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="099c7-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="099c7-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="099c7-150">Response</span></span>
<span data-ttu-id="099c7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="099c7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
