---
title: 'RangeSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7979033ce520f0d29172a910f4935c428bee383f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523579"
---
# <a name="rangesort-apply"></a><span data-ttu-id="09a4a-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="09a4a-103">RangeSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09a4a-104">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="09a4a-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="09a4a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="09a4a-105">Permissions</span></span>
<span data-ttu-id="09a4a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09a4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09a4a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09a4a-108">Permission type</span></span>      | <span data-ttu-id="09a4a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09a4a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09a4a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09a4a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="09a4a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09a4a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="09a4a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09a4a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09a4a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09a4a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="09a4a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09a4a-114">Application</span></span> | <span data-ttu-id="09a4a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09a4a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09a4a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09a4a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="09a4a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09a4a-117">Request headers</span></span>
| <span data-ttu-id="09a4a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="09a4a-118">Name</span></span>       | <span data-ttu-id="09a4a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="09a4a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="09a4a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="09a4a-120">Authorization</span></span>  | <span data-ttu-id="09a4a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09a4a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09a4a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="09a4a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="09a4a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="09a4a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09a4a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09a4a-126">Request body</span></span>
<span data-ttu-id="09a4a-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09a4a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09a4a-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="09a4a-128">Parameter</span></span>    | <span data-ttu-id="09a4a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="09a4a-129">Type</span></span>   |<span data-ttu-id="09a4a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="09a4a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09a4a-131">campos</span><span class="sxs-lookup"><span data-stu-id="09a4a-131">fields</span></span>|<span data-ttu-id="09a4a-132">SortField</span><span class="sxs-lookup"><span data-stu-id="09a4a-132">SortField</span></span>|<span data-ttu-id="09a4a-133">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="09a4a-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="09a4a-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="09a4a-134">matchCase</span></span>|<span data-ttu-id="09a4a-135">booliano</span><span class="sxs-lookup"><span data-stu-id="09a4a-135">boolean</span></span>|<span data-ttu-id="09a4a-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="09a4a-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="09a4a-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="09a4a-138">hasHeaders</span></span>|<span data-ttu-id="09a4a-139">booliano</span><span class="sxs-lookup"><span data-stu-id="09a4a-139">boolean</span></span>|<span data-ttu-id="09a4a-p105">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="09a4a-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="09a4a-142">orientation</span><span class="sxs-lookup"><span data-stu-id="09a4a-142">orientation</span></span>|<span data-ttu-id="09a4a-143">string</span><span class="sxs-lookup"><span data-stu-id="09a4a-143">string</span></span>|<span data-ttu-id="09a4a-p106">Opcional. Se a operação classifica linhas ou colunas.  Os valores possíveis são: `Rows` e `Columns`.</span><span class="sxs-lookup"><span data-stu-id="09a4a-p106">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="09a4a-147">method</span><span class="sxs-lookup"><span data-stu-id="09a4a-147">method</span></span>|<span data-ttu-id="09a4a-148">string</span><span class="sxs-lookup"><span data-stu-id="09a4a-148">string</span></span>|<span data-ttu-id="09a4a-p107">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="09a4a-p107">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="09a4a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="09a4a-152">Response</span></span>

<span data-ttu-id="09a4a-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09a4a-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09a4a-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09a4a-155">Example</span></span>
<span data-ttu-id="09a4a-156">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="09a4a-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="09a4a-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09a4a-157">Request</span></span>
<span data-ttu-id="09a4a-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09a4a-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="09a4a-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="09a4a-159">Response</span></span>
<span data-ttu-id="09a4a-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09a4a-160">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangesort-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
