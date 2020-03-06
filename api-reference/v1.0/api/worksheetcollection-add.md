---
title: 'WorksheetCollection: add'
description: . Activate () nele.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 49ba6dbe849cf027e123f5540a72b7b1da11f7f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508608"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="525e5-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="525e5-103">WorksheetCollection: add</span></span>

<span data-ttu-id="525e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="525e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="525e5-105">Adiciona uma nova planilha à pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="525e5-105">Adds a new worksheet to the workbook.</span></span> <span data-ttu-id="525e5-106">A planilha será adicionada ao final das planilhas existentes.</span><span class="sxs-lookup"><span data-stu-id="525e5-106">The worksheet will be added at the end of existing worksheets.</span></span> <span data-ttu-id="525e5-107">Se você deseja ativar a planilha recém-adicionada, chame. Activate () nele.</span><span class="sxs-lookup"><span data-stu-id="525e5-107">If you wish to activate the newly added worksheet, call .activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="525e5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="525e5-108">Permissions</span></span>
<span data-ttu-id="525e5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="525e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="525e5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="525e5-111">Permission type</span></span>      | <span data-ttu-id="525e5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="525e5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="525e5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="525e5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="525e5-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="525e5-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="525e5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="525e5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="525e5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="525e5-116">Not supported.</span></span>    |
|<span data-ttu-id="525e5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="525e5-117">Application</span></span> | <span data-ttu-id="525e5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="525e5-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="525e5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="525e5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="525e5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="525e5-120">Request headers</span></span>
| <span data-ttu-id="525e5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="525e5-121">Name</span></span>       | <span data-ttu-id="525e5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="525e5-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="525e5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="525e5-123">Authorization</span></span>  | <span data-ttu-id="525e5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="525e5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="525e5-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="525e5-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="525e5-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="525e5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="525e5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="525e5-129">Request body</span></span>
<span data-ttu-id="525e5-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="525e5-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="525e5-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="525e5-131">Parameter</span></span>    | <span data-ttu-id="525e5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="525e5-132">Type</span></span>   |<span data-ttu-id="525e5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="525e5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="525e5-134">nome</span><span class="sxs-lookup"><span data-stu-id="525e5-134">name</span></span>|<span data-ttu-id="525e5-135">string</span><span class="sxs-lookup"><span data-stu-id="525e5-135">string</span></span>|<span data-ttu-id="525e5-p105">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="525e5-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="525e5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="525e5-140">Response</span></span>

<span data-ttu-id="525e5-141">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookWorksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="525e5-141">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="525e5-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="525e5-142">Example</span></span>
<span data-ttu-id="525e5-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="525e5-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="525e5-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="525e5-144">Request</span></span>
<span data-ttu-id="525e5-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="525e5-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="525e5-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="525e5-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="525e5-147">C#</span><span class="sxs-lookup"><span data-stu-id="525e5-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="525e5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="525e5-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="525e5-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="525e5-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="525e5-150">Java</span><span class="sxs-lookup"><span data-stu-id="525e5-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="525e5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="525e5-151">Response</span></span>
<span data-ttu-id="525e5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="525e5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
