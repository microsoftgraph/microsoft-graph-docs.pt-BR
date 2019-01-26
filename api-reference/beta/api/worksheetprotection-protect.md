---
title: 'WorksheetProtection: protect'
description: Protege uma planilha. Gera uma exceção se a planilha estiver protegida.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bb02bfd77cd1e86f6acf9b4f2f393474f484b11
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572952"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="71b87-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="71b87-104">WorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71b87-p102">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="71b87-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="71b87-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="71b87-107">Permissions</span></span>
<span data-ttu-id="71b87-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71b87-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71b87-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71b87-110">Permission type</span></span>      | <span data-ttu-id="71b87-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71b87-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71b87-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71b87-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71b87-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71b87-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71b87-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71b87-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b87-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71b87-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71b87-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71b87-116">Application</span></span> | <span data-ttu-id="71b87-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71b87-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71b87-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71b87-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="71b87-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71b87-119">Request headers</span></span>
| <span data-ttu-id="71b87-120">Nome</span><span class="sxs-lookup"><span data-stu-id="71b87-120">Name</span></span>       | <span data-ttu-id="71b87-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="71b87-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71b87-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="71b87-122">Authorization</span></span>  | <span data-ttu-id="71b87-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71b87-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71b87-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71b87-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="71b87-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="71b87-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71b87-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71b87-128">Request body</span></span>
<span data-ttu-id="71b87-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71b87-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71b87-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="71b87-130">Parameter</span></span>    | <span data-ttu-id="71b87-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="71b87-131">Type</span></span>   |<span data-ttu-id="71b87-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="71b87-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71b87-133">options</span><span class="sxs-lookup"><span data-stu-id="71b87-133">options</span></span>|<span data-ttu-id="71b87-134">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="71b87-134">workbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="71b87-p106">Opcional. Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="71b87-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="71b87-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="71b87-137">Response</span></span>

<span data-ttu-id="71b87-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71b87-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71b87-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71b87-140">Example</span></span>
<span data-ttu-id="71b87-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="71b87-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="71b87-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71b87-142">Request</span></span>
<span data-ttu-id="71b87-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71b87-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="71b87-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="71b87-144">Response</span></span>
<span data-ttu-id="71b87-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71b87-145">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetprotection-protect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
