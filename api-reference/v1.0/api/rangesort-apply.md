---
title: 'RangeSort: apply'
description: Execute uma operação de classificação.
ms.openlocfilehash: 76432fb2614d92f5f3acbdc2261712085db5ec83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005648"
---
# <a name="rangesort-apply"></a><span data-ttu-id="0bc3b-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="0bc3b-103">RangeSort: apply</span></span>

<span data-ttu-id="0bc3b-104">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="0bc3b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0bc3b-105">Permissions</span></span>
<span data-ttu-id="0bc3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bc3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bc3b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bc3b-108">Permission type</span></span>      | <span data-ttu-id="0bc3b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0bc3b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bc3b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bc3b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0bc3b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0bc3b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0bc3b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bc3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bc3b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-113">Not supported.</span></span>    |
|<span data-ttu-id="0bc3b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bc3b-114">Application</span></span> | <span data-ttu-id="0bc3b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bc3b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bc3b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="0bc3b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc3b-117">Request headers</span></span>
| <span data-ttu-id="0bc3b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0bc3b-118">Name</span></span>       | <span data-ttu-id="0bc3b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc3b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0bc3b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bc3b-120">Authorization</span></span>  | <span data-ttu-id="0bc3b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bc3b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0bc3b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0bc3b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bc3b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc3b-126">Request body</span></span>
<span data-ttu-id="0bc3b-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0bc3b-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0bc3b-128">Parameter</span></span>    | <span data-ttu-id="0bc3b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bc3b-129">Type</span></span>   |<span data-ttu-id="0bc3b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc3b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bc3b-131">campos</span><span class="sxs-lookup"><span data-stu-id="0bc3b-131">fields</span></span>|<span data-ttu-id="0bc3b-132">Coleção WorkbookSortField</span><span class="sxs-lookup"><span data-stu-id="0bc3b-132">WorkbookSortField collection</span></span>|<span data-ttu-id="0bc3b-133">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="0bc3b-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="0bc3b-134">matchCase</span></span>|<span data-ttu-id="0bc3b-135">booliano</span><span class="sxs-lookup"><span data-stu-id="0bc3b-135">boolean</span></span>|<span data-ttu-id="0bc3b-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="0bc3b-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="0bc3b-138">hasHeaders</span></span>|<span data-ttu-id="0bc3b-139">booliano</span><span class="sxs-lookup"><span data-stu-id="0bc3b-139">boolean</span></span>|<span data-ttu-id="0bc3b-p105">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="0bc3b-142">orientation</span><span class="sxs-lookup"><span data-stu-id="0bc3b-142">orientation</span></span>|<span data-ttu-id="0bc3b-143">string</span><span class="sxs-lookup"><span data-stu-id="0bc3b-143">string</span></span>|<span data-ttu-id="0bc3b-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-144">Optional.</span></span> <span data-ttu-id="0bc3b-145">Se a operação é classificando linhas ou colunas.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="0bc3b-146">Os valores possíveis são: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="0bc3b-147">method</span><span class="sxs-lookup"><span data-stu-id="0bc3b-147">method</span></span>|<span data-ttu-id="0bc3b-148">string</span><span class="sxs-lookup"><span data-stu-id="0bc3b-148">string</span></span>|<span data-ttu-id="0bc3b-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-149">Optional.</span></span> <span data-ttu-id="0bc3b-150">O método de ordenação usado para caracteres chineses.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="0bc3b-151">Os valores possíveis são: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="0bc3b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bc3b-152">Response</span></span>

<span data-ttu-id="0bc3b-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bc3b-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bc3b-155">Example</span></span>
<span data-ttu-id="0bc3b-156">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0bc3b-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc3b-157">Request</span></span>
<span data-ttu-id="0bc3b-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
Content-type: application/json
Content-length: 358

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="0bc3b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bc3b-159">Response</span></span>
<span data-ttu-id="0bc3b-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bc3b-160">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->