---
title: Adicionar Item nomeado
description: Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: df9279c091fd2c69a95ebfad72dbee0aa472079b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576222"
---
# <a name="add-named-item"></a><span data-ttu-id="80ec2-103">Adicionar Item nomeado</span><span class="sxs-lookup"><span data-stu-id="80ec2-103">Add Named Item</span></span>

<span data-ttu-id="80ec2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80ec2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80ec2-105">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="80ec2-105">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="80ec2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="80ec2-106">Permissions</span></span>
<span data-ttu-id="80ec2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80ec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80ec2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80ec2-109">Permission type</span></span>      | <span data-ttu-id="80ec2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80ec2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80ec2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80ec2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="80ec2-112">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="80ec2-112">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="80ec2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80ec2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80ec2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80ec2-114">Not supported.</span></span>    |
|<span data-ttu-id="80ec2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80ec2-115">Application</span></span> | <span data-ttu-id="80ec2-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="80ec2-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80ec2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80ec2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/add
POST /me/drive/root:/{item-path}:/workbook/names/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/names/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="80ec2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80ec2-118">Request headers</span></span>
| <span data-ttu-id="80ec2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="80ec2-119">Name</span></span>       | <span data-ttu-id="80ec2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="80ec2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="80ec2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="80ec2-121">Authorization</span></span>  | <span data-ttu-id="80ec2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80ec2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80ec2-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="80ec2-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="80ec2-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="80ec2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80ec2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80ec2-127">Request body</span></span>
<span data-ttu-id="80ec2-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80ec2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="80ec2-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="80ec2-129">Parameter</span></span>    | <span data-ttu-id="80ec2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="80ec2-130">Type</span></span>   |<span data-ttu-id="80ec2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="80ec2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80ec2-132">nome</span><span class="sxs-lookup"><span data-stu-id="80ec2-132">name</span></span>|<span data-ttu-id="80ec2-133">string</span><span class="sxs-lookup"><span data-stu-id="80ec2-133">string</span></span>|<span data-ttu-id="80ec2-134">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="80ec2-134">The name of the named item.</span></span>|
|<span data-ttu-id="80ec2-135">de referência</span><span class="sxs-lookup"><span data-stu-id="80ec2-135">reference</span></span>|<span data-ttu-id="80ec2-136">Json</span><span class="sxs-lookup"><span data-stu-id="80ec2-136">Json</span></span>|<span data-ttu-id="80ec2-137">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="80ec2-137">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="80ec2-138">comment</span><span class="sxs-lookup"><span data-stu-id="80ec2-138">comment</span></span>|<span data-ttu-id="80ec2-139">string</span><span class="sxs-lookup"><span data-stu-id="80ec2-139">string</span></span>|<span data-ttu-id="80ec2-140">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="80ec2-140">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="80ec2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ec2-141">Response</span></span>

<span data-ttu-id="80ec2-142">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [WorkbookNamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80ec2-142">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="80ec2-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80ec2-143">Example</span></span>
<span data-ttu-id="80ec2-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="80ec2-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="80ec2-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80ec2-145">Request</span></span>
<span data-ttu-id="80ec2-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80ec2-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80ec2-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="80ec2-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="80ec2-148">C#</span><span class="sxs-lookup"><span data-stu-id="80ec2-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80ec2-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80ec2-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80ec2-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80ec2-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80ec2-151">Java</span><span class="sxs-lookup"><span data-stu-id="80ec2-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="80ec2-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ec2-152">Response</span></span>
<span data-ttu-id="80ec2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80ec2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

