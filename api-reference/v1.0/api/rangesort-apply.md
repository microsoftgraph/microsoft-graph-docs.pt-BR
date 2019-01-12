---
title: 'RangeSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be024f3eacbb4e2d1178ec7b82a8e8ca604aff60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967102"
---
# <a name="rangesort-apply"></a><span data-ttu-id="27aa9-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="27aa9-103">RangeSort: apply</span></span>

<span data-ttu-id="27aa9-104">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="27aa9-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="27aa9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="27aa9-105">Permissions</span></span>
<span data-ttu-id="27aa9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27aa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27aa9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27aa9-108">Permission type</span></span>      | <span data-ttu-id="27aa9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27aa9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27aa9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27aa9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27aa9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27aa9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="27aa9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27aa9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27aa9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27aa9-113">Not supported.</span></span>    |
|<span data-ttu-id="27aa9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27aa9-114">Application</span></span> | <span data-ttu-id="27aa9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27aa9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27aa9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27aa9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="27aa9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27aa9-117">Request headers</span></span>
| <span data-ttu-id="27aa9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="27aa9-118">Name</span></span>       | <span data-ttu-id="27aa9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="27aa9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="27aa9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="27aa9-120">Authorization</span></span>  | <span data-ttu-id="27aa9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27aa9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27aa9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="27aa9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="27aa9-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="27aa9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27aa9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27aa9-126">Request body</span></span>
<span data-ttu-id="27aa9-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27aa9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="27aa9-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="27aa9-128">Parameter</span></span>    | <span data-ttu-id="27aa9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="27aa9-129">Type</span></span>   |<span data-ttu-id="27aa9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="27aa9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27aa9-131">campos</span><span class="sxs-lookup"><span data-stu-id="27aa9-131">fields</span></span>|<span data-ttu-id="27aa9-132">Coleção WorkbookSortField</span><span class="sxs-lookup"><span data-stu-id="27aa9-132">WorkbookSortField collection</span></span>|<span data-ttu-id="27aa9-133">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="27aa9-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="27aa9-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="27aa9-134">matchCase</span></span>|<span data-ttu-id="27aa9-135">booliano</span><span class="sxs-lookup"><span data-stu-id="27aa9-135">boolean</span></span>|<span data-ttu-id="27aa9-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="27aa9-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="27aa9-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="27aa9-138">hasHeaders</span></span>|<span data-ttu-id="27aa9-139">booliano</span><span class="sxs-lookup"><span data-stu-id="27aa9-139">boolean</span></span>|<span data-ttu-id="27aa9-p105">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="27aa9-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="27aa9-142">orientation</span><span class="sxs-lookup"><span data-stu-id="27aa9-142">orientation</span></span>|<span data-ttu-id="27aa9-143">string</span><span class="sxs-lookup"><span data-stu-id="27aa9-143">string</span></span>|<span data-ttu-id="27aa9-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="27aa9-144">Optional.</span></span> <span data-ttu-id="27aa9-145">Se a operação é classificando linhas ou colunas.</span><span class="sxs-lookup"><span data-stu-id="27aa9-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="27aa9-146">Os valores possíveis são: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="27aa9-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="27aa9-147">method</span><span class="sxs-lookup"><span data-stu-id="27aa9-147">method</span></span>|<span data-ttu-id="27aa9-148">string</span><span class="sxs-lookup"><span data-stu-id="27aa9-148">string</span></span>|<span data-ttu-id="27aa9-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="27aa9-149">Optional.</span></span> <span data-ttu-id="27aa9-150">O método de ordenação usado para caracteres chineses.</span><span class="sxs-lookup"><span data-stu-id="27aa9-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="27aa9-151">Os valores possíveis são: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="27aa9-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="27aa9-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="27aa9-152">Response</span></span>

<span data-ttu-id="27aa9-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27aa9-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27aa9-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27aa9-155">Example</span></span>
<span data-ttu-id="27aa9-156">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="27aa9-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="27aa9-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27aa9-157">Request</span></span>
<span data-ttu-id="27aa9-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27aa9-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="27aa9-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="27aa9-159">Response</span></span>
<span data-ttu-id="27aa9-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27aa9-160">Here is an example of the response.</span></span> 
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
