---
title: 'workbookWorksheetProtection: proteger'
description: Protege uma planilha. Gera uma exceção se a planilha estiver protegida.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b10fa4454b5937c2548e023adfd34900a16c8c95
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339367"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="63c15-104">workbookWorksheetProtection: proteger</span><span class="sxs-lookup"><span data-stu-id="63c15-104">workbookWorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63c15-105">Protege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="63c15-105">Protect a worksheet.</span></span> <span data-ttu-id="63c15-106">Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="63c15-106">It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="63c15-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="63c15-107">Permissions</span></span>
<span data-ttu-id="63c15-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63c15-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63c15-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63c15-110">Permission type</span></span>      | <span data-ttu-id="63c15-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63c15-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63c15-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63c15-112">Delegated (work or school account)</span></span> | <span data-ttu-id="63c15-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63c15-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63c15-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63c15-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63c15-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63c15-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63c15-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63c15-116">Application</span></span> | <span data-ttu-id="63c15-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63c15-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63c15-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63c15-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="63c15-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63c15-119">Request headers</span></span>
| <span data-ttu-id="63c15-120">Nome</span><span class="sxs-lookup"><span data-stu-id="63c15-120">Name</span></span>       | <span data-ttu-id="63c15-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="63c15-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63c15-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63c15-122">Authorization</span></span>  | <span data-ttu-id="63c15-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63c15-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63c15-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="63c15-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="63c15-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="63c15-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63c15-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63c15-128">Request body</span></span>
<span data-ttu-id="63c15-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63c15-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63c15-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="63c15-130">Parameter</span></span>    | <span data-ttu-id="63c15-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="63c15-131">Type</span></span>   |<span data-ttu-id="63c15-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="63c15-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63c15-133">options</span><span class="sxs-lookup"><span data-stu-id="63c15-133">options</span></span>|[<span data-ttu-id="63c15-134">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="63c15-134">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="63c15-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63c15-135">Optional.</span></span> <span data-ttu-id="63c15-136">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="63c15-136">sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="63c15-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="63c15-137">Response</span></span>

<span data-ttu-id="63c15-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63c15-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63c15-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63c15-140">Example</span></span>
<span data-ttu-id="63c15-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="63c15-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="63c15-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63c15-142">Request</span></span>
<span data-ttu-id="63c15-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63c15-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookworksheetprotection_protect"
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

##### <a name="response"></a><span data-ttu-id="63c15-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="63c15-144">Response</span></span>
<span data-ttu-id="63c15-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63c15-145">Here is an example of the response.</span></span> 
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
  "description": "workbookWorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
