---
title: Adicionar Item nomeado
description: Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 861827d29b406778c4770f026d319131f75fd99a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062390"
---
# <a name="add-named-item"></a><span data-ttu-id="3ef7c-103">Adicionar Item nomeado</span><span class="sxs-lookup"><span data-stu-id="3ef7c-103">Add Named Item</span></span>

<span data-ttu-id="3ef7c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ef7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ef7c-105">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-105">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ef7c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ef7c-106">Permissions</span></span>
<span data-ttu-id="3ef7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ef7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ef7c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ef7c-109">Permission type</span></span>      | <span data-ttu-id="3ef7c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ef7c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ef7c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ef7c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ef7c-112">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ef7c-112">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="3ef7c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ef7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ef7c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ef7c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3ef7c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ef7c-115">Application</span></span> | <span data-ttu-id="3ef7c-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ef7c-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ef7c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef7c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="3ef7c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef7c-118">Request headers</span></span>
| <span data-ttu-id="3ef7c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3ef7c-119">Name</span></span>       | <span data-ttu-id="3ef7c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ef7c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3ef7c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ef7c-121">Authorization</span></span>  | <span data-ttu-id="3ef7c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ef7c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3ef7c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3ef7c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ef7c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef7c-127">Request body</span></span>
<span data-ttu-id="3ef7c-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ef7c-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3ef7c-129">Parameter</span></span>    | <span data-ttu-id="3ef7c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ef7c-130">Type</span></span>   |<span data-ttu-id="3ef7c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ef7c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ef7c-132">name</span><span class="sxs-lookup"><span data-stu-id="3ef7c-132">name</span></span>|<span data-ttu-id="3ef7c-133">string</span><span class="sxs-lookup"><span data-stu-id="3ef7c-133">string</span></span>|<span data-ttu-id="3ef7c-134">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-134">The name of the named item.</span></span>|
|<span data-ttu-id="3ef7c-135">reference</span><span class="sxs-lookup"><span data-stu-id="3ef7c-135">reference</span></span>|<span data-ttu-id="3ef7c-136">string</span><span class="sxs-lookup"><span data-stu-id="3ef7c-136">string</span></span>|<span data-ttu-id="3ef7c-137">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-137">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="3ef7c-138">comment</span><span class="sxs-lookup"><span data-stu-id="3ef7c-138">comment</span></span>|<span data-ttu-id="3ef7c-139">string</span><span class="sxs-lookup"><span data-stu-id="3ef7c-139">string</span></span>|<span data-ttu-id="3ef7c-140">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="3ef7c-140">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="3ef7c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef7c-141">Response</span></span>

<span data-ttu-id="3ef7c-142">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [workbookNamedItem](../resources/workbooknameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-142">If successful, this method returns `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ef7c-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ef7c-143">Example</span></span>
<span data-ttu-id="3ef7c-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3ef7c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef7c-145">Request</span></span>
<span data-ttu-id="3ef7c-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ef7c-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef7c-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```
# <a name="c"></a>[<span data-ttu-id="3ef7c-148">C#</span><span class="sxs-lookup"><span data-stu-id="3ef7c-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef7c-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef7c-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef7c-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef7c-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3ef7c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef7c-151">Response</span></span>
<span data-ttu-id="3ef7c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef7c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


