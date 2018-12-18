---
title: 'TableSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
ms.openlocfilehash: d3e19dbd1ed77f32a215dfa165ebc796706b09a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309678"
---
# <a name="tablesort-apply"></a><span data-ttu-id="a089f-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="a089f-103">TableSort: apply</span></span>

<span data-ttu-id="a089f-104">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="a089f-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="a089f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a089f-105">Permissions</span></span>
<span data-ttu-id="a089f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a089f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a089f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a089f-108">Permission type</span></span>      | <span data-ttu-id="a089f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a089f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a089f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a089f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a089f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a089f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a089f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a089f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a089f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a089f-113">Not supported.</span></span>    |
|<span data-ttu-id="a089f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a089f-114">Application</span></span> | <span data-ttu-id="a089f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a089f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a089f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a089f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="a089f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a089f-117">Request headers</span></span>
| <span data-ttu-id="a089f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a089f-118">Name</span></span>       | <span data-ttu-id="a089f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a089f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a089f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a089f-120">Authorization</span></span>  | <span data-ttu-id="a089f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a089f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a089f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a089f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a089f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a089f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a089f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a089f-126">Request body</span></span>
<span data-ttu-id="a089f-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a089f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a089f-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a089f-128">Parameter</span></span>    | <span data-ttu-id="a089f-129">Type</span><span class="sxs-lookup"><span data-stu-id="a089f-129">Type</span></span>   |<span data-ttu-id="a089f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a089f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a089f-131">campos</span><span class="sxs-lookup"><span data-stu-id="a089f-131">fields</span></span>|<span data-ttu-id="a089f-132">Coleção WorkbookSortField</span><span class="sxs-lookup"><span data-stu-id="a089f-132">WorkbookSortField collection</span></span>|<span data-ttu-id="a089f-133">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="a089f-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="a089f-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="a089f-134">matchCase</span></span>|<span data-ttu-id="a089f-135">booliano</span><span class="sxs-lookup"><span data-stu-id="a089f-135">boolean</span></span>|<span data-ttu-id="a089f-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="a089f-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="a089f-138">method</span><span class="sxs-lookup"><span data-stu-id="a089f-138">method</span></span>|<span data-ttu-id="a089f-139">string</span><span class="sxs-lookup"><span data-stu-id="a089f-139">string</span></span>|<span data-ttu-id="a089f-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a089f-140">Optional.</span></span> <span data-ttu-id="a089f-141">O método de ordenação usado para caracteres chineses.</span><span class="sxs-lookup"><span data-stu-id="a089f-141">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="a089f-142">Os valores possíveis são: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="a089f-142">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="a089f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a089f-143">Response</span></span>

<span data-ttu-id="a089f-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a089f-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a089f-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a089f-146">Example</span></span>
<span data-ttu-id="a089f-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a089f-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a089f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a089f-148">Request</span></span>
<span data-ttu-id="a089f-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a089f-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

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
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="a089f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a089f-150">Response</span></span>
<span data-ttu-id="a089f-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a089f-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->