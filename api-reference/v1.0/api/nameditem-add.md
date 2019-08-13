---
title: Adicionar Item nomeado
description: Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: a9392346c3f3a3e09c2fe1a3a4627c1304919a8e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374608"
---
# <a name="add-named-item"></a><span data-ttu-id="7429c-103">Adicionar Item nomeado</span><span class="sxs-lookup"><span data-stu-id="7429c-103">Add Named Item</span></span>

<span data-ttu-id="7429c-104">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="7429c-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="7429c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7429c-105">Permissions</span></span>
<span data-ttu-id="7429c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7429c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7429c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7429c-108">Permission type</span></span>      | <span data-ttu-id="7429c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7429c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7429c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7429c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7429c-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="7429c-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="7429c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7429c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7429c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7429c-113">Not supported.</span></span>    |
|<span data-ttu-id="7429c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7429c-114">Application</span></span> | <span data-ttu-id="7429c-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="7429c-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7429c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7429c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="7429c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7429c-117">Request headers</span></span>
| <span data-ttu-id="7429c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7429c-118">Name</span></span>       | <span data-ttu-id="7429c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7429c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7429c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7429c-120">Authorization</span></span>  | <span data-ttu-id="7429c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7429c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7429c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7429c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7429c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7429c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7429c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7429c-126">Request body</span></span>
<span data-ttu-id="7429c-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7429c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7429c-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7429c-128">Parameter</span></span>    | <span data-ttu-id="7429c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7429c-129">Type</span></span>   |<span data-ttu-id="7429c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7429c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7429c-131">name</span><span class="sxs-lookup"><span data-stu-id="7429c-131">name</span></span>|<span data-ttu-id="7429c-132">string</span><span class="sxs-lookup"><span data-stu-id="7429c-132">string</span></span>|<span data-ttu-id="7429c-133">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="7429c-133">The name of the named item.</span></span>|
|<span data-ttu-id="7429c-134">de referência</span><span class="sxs-lookup"><span data-stu-id="7429c-134">reference</span></span>|<span data-ttu-id="7429c-135">Json</span><span class="sxs-lookup"><span data-stu-id="7429c-135">Json</span></span>|<span data-ttu-id="7429c-136">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="7429c-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="7429c-137">comentário</span><span class="sxs-lookup"><span data-stu-id="7429c-137">comment</span></span>|<span data-ttu-id="7429c-138">string</span><span class="sxs-lookup"><span data-stu-id="7429c-138">string</span></span>|<span data-ttu-id="7429c-139">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="7429c-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="7429c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7429c-140">Response</span></span>

<span data-ttu-id="7429c-141">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookNamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7429c-141">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="7429c-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7429c-142">Example</span></span>
<span data-ttu-id="7429c-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7429c-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7429c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7429c-144">Request</span></span>
<span data-ttu-id="7429c-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7429c-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7429c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="7429c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7429c-147">C#</span><span class="sxs-lookup"><span data-stu-id="7429c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7429c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7429c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7429c-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7429c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7429c-150">Java</span><span class="sxs-lookup"><span data-stu-id="7429c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7429c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7429c-151">Response</span></span>
<span data-ttu-id="7429c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7429c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
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
  "suppressions": [
    "Warning: NamedItemcollection_add/value:
      Schemas type was 'Custom' which is not supported. Add a resource type to the definition of property: value"
  ],
  "tocPath": ""
}-->
