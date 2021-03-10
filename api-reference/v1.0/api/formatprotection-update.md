---
title: Atualizar formatprotection
description: Atualiza as propriedades do objeto formatprotection.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 43f7b9f1c0f7e8885f871b7e760a78e866a4cf0f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573695"
---
# <a name="update-formatprotection"></a><span data-ttu-id="6b998-103">Atualizar formatprotection</span><span class="sxs-lookup"><span data-stu-id="6b998-103">Update formatprotection</span></span>

<span data-ttu-id="6b998-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b998-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b998-105">Atualiza as propriedades do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="6b998-105">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b998-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b998-106">Permissions</span></span>
<span data-ttu-id="6b998-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b998-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b998-109">Permission type</span></span>      | <span data-ttu-id="6b998-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b998-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b998-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b998-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b998-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b998-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b998-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b998-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b998-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b998-114">Not supported.</span></span>    |
|<span data-ttu-id="6b998-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b998-115">Application</span></span> | <span data-ttu-id="6b998-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b998-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b998-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b998-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/protection
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/protection
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="6b998-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="6b998-118">Optional request headers</span></span>
| <span data-ttu-id="6b998-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b998-119">Name</span></span>       | <span data-ttu-id="6b998-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b998-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6b998-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b998-121">Authorization</span></span>  | <span data-ttu-id="6b998-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b998-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6b998-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b998-124">Request body</span></span>
<span data-ttu-id="6b998-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6b998-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6b998-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b998-128">Property</span></span>     | <span data-ttu-id="6b998-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b998-129">Type</span></span>   |<span data-ttu-id="6b998-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b998-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b998-131">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="6b998-131">formulaHidden</span></span>|<span data-ttu-id="6b998-132">booliano</span><span class="sxs-lookup"><span data-stu-id="6b998-132">boolean</span></span>|<span data-ttu-id="6b998-p104">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="6b998-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="6b998-135">locked</span><span class="sxs-lookup"><span data-stu-id="6b998-135">locked</span></span>|<span data-ttu-id="6b998-136">booliano</span><span class="sxs-lookup"><span data-stu-id="6b998-136">boolean</span></span>|<span data-ttu-id="6b998-p105">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="6b998-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="6b998-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b998-139">Response</span></span>

<span data-ttu-id="6b998-140">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b998-140">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b998-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b998-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b998-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b998-142">Request</span></span>
<span data-ttu-id="6b998-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b998-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b998-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b998-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
# <a name="c"></a>[<span data-ttu-id="6b998-145">C#</span><span class="sxs-lookup"><span data-stu-id="6b998-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b998-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b998-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b998-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b998-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b998-148">Java</span><span class="sxs-lookup"><span data-stu-id="6b998-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b998-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b998-149">Response</span></span>
<span data-ttu-id="6b998-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b998-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

