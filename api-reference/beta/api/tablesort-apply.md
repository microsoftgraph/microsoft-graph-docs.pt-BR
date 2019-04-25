---
title: 'TableSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f2279109f83758958cb00940604854c4edeecd45
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544565"
---
# <a name="tablesort-apply"></a><span data-ttu-id="01616-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="01616-103">TableSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01616-104">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="01616-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="01616-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="01616-105">Permissions</span></span>
<span data-ttu-id="01616-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01616-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01616-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01616-108">Permission type</span></span>      | <span data-ttu-id="01616-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01616-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01616-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01616-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01616-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01616-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01616-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01616-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01616-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01616-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01616-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01616-114">Application</span></span> | <span data-ttu-id="01616-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01616-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01616-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01616-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="01616-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01616-117">Request headers</span></span>
| <span data-ttu-id="01616-118">Nome</span><span class="sxs-lookup"><span data-stu-id="01616-118">Name</span></span>       | <span data-ttu-id="01616-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="01616-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01616-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="01616-120">Authorization</span></span>  | <span data-ttu-id="01616-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01616-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01616-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="01616-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="01616-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="01616-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01616-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01616-126">Request body</span></span>
<span data-ttu-id="01616-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01616-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01616-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="01616-128">Parameter</span></span>    | <span data-ttu-id="01616-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="01616-129">Type</span></span>   |<span data-ttu-id="01616-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="01616-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01616-131">campos</span><span class="sxs-lookup"><span data-stu-id="01616-131">fields</span></span>|<span data-ttu-id="01616-132">SortField</span><span class="sxs-lookup"><span data-stu-id="01616-132">SortField</span></span>|<span data-ttu-id="01616-133">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="01616-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="01616-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="01616-134">matchCase</span></span>|<span data-ttu-id="01616-135">booliano</span><span class="sxs-lookup"><span data-stu-id="01616-135">boolean</span></span>|<span data-ttu-id="01616-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="01616-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="01616-138">method</span><span class="sxs-lookup"><span data-stu-id="01616-138">method</span></span>|<span data-ttu-id="01616-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01616-139">string</span></span>|<span data-ttu-id="01616-p105">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="01616-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="01616-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="01616-143">Response</span></span>

<span data-ttu-id="01616-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01616-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01616-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01616-146">Example</span></span>
<span data-ttu-id="01616-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="01616-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="01616-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01616-148">Request</span></span>
<span data-ttu-id="01616-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01616-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
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

##### <a name="response"></a><span data-ttu-id="01616-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="01616-150">Response</span></span>
<span data-ttu-id="01616-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01616-151">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablesort-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
