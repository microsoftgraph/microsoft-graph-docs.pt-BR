---
title: 'WorksheetCollection: add'
description: .activate() nele.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a4c587117beeb6e06e7a683dd119d8199c3e940c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578154"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="59c19-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="59c19-103">WorksheetCollection: add</span></span>

<span data-ttu-id="59c19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59c19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59c19-p101">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. Se você quiser ativar a planilha recém-adicionada, chame “.activate()” nela.</span><span class="sxs-lookup"><span data-stu-id="59c19-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="59c19-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="59c19-108">Permissions</span></span>
<span data-ttu-id="59c19-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59c19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59c19-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59c19-111">Permission type</span></span>      | <span data-ttu-id="59c19-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59c19-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59c19-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59c19-113">Delegated (work or school account)</span></span> | <span data-ttu-id="59c19-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59c19-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59c19-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59c19-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59c19-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59c19-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59c19-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59c19-117">Application</span></span> | <span data-ttu-id="59c19-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59c19-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59c19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59c19-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/
POST /me/drive/root:/{item-path}:/workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="59c19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59c19-120">Request headers</span></span>
| <span data-ttu-id="59c19-121">Nome</span><span class="sxs-lookup"><span data-stu-id="59c19-121">Name</span></span>       | <span data-ttu-id="59c19-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c19-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59c19-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59c19-123">Authorization</span></span>  | <span data-ttu-id="59c19-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59c19-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59c19-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="59c19-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="59c19-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="59c19-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59c19-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59c19-129">Request body</span></span>
<span data-ttu-id="59c19-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59c19-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59c19-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59c19-131">Parameter</span></span>    | <span data-ttu-id="59c19-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="59c19-132">Type</span></span>   |<span data-ttu-id="59c19-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c19-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59c19-134">nome</span><span class="sxs-lookup"><span data-stu-id="59c19-134">name</span></span>|<span data-ttu-id="59c19-135">string</span><span class="sxs-lookup"><span data-stu-id="59c19-135">string</span></span>|<span data-ttu-id="59c19-p105">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="59c19-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="59c19-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="59c19-140">Response</span></span>

<span data-ttu-id="59c19-141">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [workbookWorksheet](../resources/workbookworksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59c19-141">If successful, this method returns `200 OK` response code and [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59c19-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59c19-142">Example</span></span>
<span data-ttu-id="59c19-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="59c19-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="59c19-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59c19-144">Request</span></span>
<span data-ttu-id="59c19-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59c19-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59c19-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="59c19-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="59c19-147">C#</span><span class="sxs-lookup"><span data-stu-id="59c19-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59c19-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59c19-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59c19-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59c19-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59c19-150">Java</span><span class="sxs-lookup"><span data-stu-id="59c19-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59c19-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="59c19-151">Response</span></span>
<span data-ttu-id="59c19-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59c19-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


