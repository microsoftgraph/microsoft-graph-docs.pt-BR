---
title: 'RangeSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 66006bafdc26ecca85dda3dc0eb0999a387dddc5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968362"
---
# <a name="rangesort-apply"></a><span data-ttu-id="e6fcd-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="e6fcd-103">RangeSort: apply</span></span>

> <span data-ttu-id="e6fcd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6fcd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6fcd-106">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6fcd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6fcd-107">Permissions</span></span>
<span data-ttu-id="e6fcd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6fcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6fcd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6fcd-110">Permission type</span></span>      | <span data-ttu-id="e6fcd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6fcd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6fcd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6fcd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6fcd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6fcd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6fcd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6fcd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6fcd-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6fcd-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6fcd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6fcd-116">Application</span></span> | <span data-ttu-id="e6fcd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6fcd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6fcd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="e6fcd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6fcd-119">Request headers</span></span>
| <span data-ttu-id="e6fcd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e6fcd-120">Name</span></span>       | <span data-ttu-id="e6fcd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6fcd-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6fcd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6fcd-122">Authorization</span></span>  | <span data-ttu-id="e6fcd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6fcd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e6fcd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e6fcd-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6fcd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6fcd-128">Request body</span></span>
<span data-ttu-id="e6fcd-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6fcd-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6fcd-130">Parameter</span></span>    | <span data-ttu-id="e6fcd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6fcd-131">Type</span></span>   |<span data-ttu-id="e6fcd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6fcd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6fcd-133">campos</span><span class="sxs-lookup"><span data-stu-id="e6fcd-133">fields</span></span>|<span data-ttu-id="e6fcd-134">SortField</span><span class="sxs-lookup"><span data-stu-id="e6fcd-134">SortField</span></span>|<span data-ttu-id="e6fcd-135">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="e6fcd-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="e6fcd-136">matchCase</span></span>|<span data-ttu-id="e6fcd-137">booliano</span><span class="sxs-lookup"><span data-stu-id="e6fcd-137">boolean</span></span>|<span data-ttu-id="e6fcd-p105">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="e6fcd-140">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="e6fcd-140">hasHeaders</span></span>|<span data-ttu-id="e6fcd-141">booliano</span><span class="sxs-lookup"><span data-stu-id="e6fcd-141">boolean</span></span>|<span data-ttu-id="e6fcd-p106">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-p106">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="e6fcd-144">orientation</span><span class="sxs-lookup"><span data-stu-id="e6fcd-144">orientation</span></span>|<span data-ttu-id="e6fcd-145">string</span><span class="sxs-lookup"><span data-stu-id="e6fcd-145">string</span></span>|<span data-ttu-id="e6fcd-p107">Opcional. Se a operação classifica linhas ou colunas.  Os valores possíveis são: `Rows` e `Columns`.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-p107">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="e6fcd-149">method</span><span class="sxs-lookup"><span data-stu-id="e6fcd-149">method</span></span>|<span data-ttu-id="e6fcd-150">string</span><span class="sxs-lookup"><span data-stu-id="e6fcd-150">string</span></span>|<span data-ttu-id="e6fcd-p108">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-p108">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="e6fcd-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6fcd-154">Response</span></span>

<span data-ttu-id="e6fcd-p109">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-p109">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6fcd-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6fcd-157">Example</span></span>
<span data-ttu-id="e6fcd-158">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6fcd-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6fcd-159">Request</span></span>
<span data-ttu-id="e6fcd-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
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

##### <a name="response"></a><span data-ttu-id="e6fcd-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6fcd-161">Response</span></span>
<span data-ttu-id="e6fcd-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6fcd-162">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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
