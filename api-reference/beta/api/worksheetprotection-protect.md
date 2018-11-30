---
title: 'WorksheetProtection: protect'
description: Protege uma planilha. Gera uma exceção se a planilha estiver protegida.
ms.openlocfilehash: 885928c592f6aafe320181e62b3993dfbdadf87e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036689"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="57a34-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="57a34-104">WorksheetProtection: protect</span></span>

> <span data-ttu-id="57a34-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="57a34-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57a34-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="57a34-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57a34-p103">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="57a34-p103">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="57a34-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="57a34-109">Permissions</span></span>
<span data-ttu-id="57a34-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57a34-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57a34-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57a34-112">Permission type</span></span>      | <span data-ttu-id="57a34-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57a34-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57a34-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57a34-114">Delegated (work or school account)</span></span> | <span data-ttu-id="57a34-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57a34-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57a34-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57a34-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57a34-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57a34-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57a34-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57a34-118">Application</span></span> | <span data-ttu-id="57a34-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57a34-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57a34-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57a34-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="57a34-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57a34-121">Request headers</span></span>
| <span data-ttu-id="57a34-122">Nome</span><span class="sxs-lookup"><span data-stu-id="57a34-122">Name</span></span>       | <span data-ttu-id="57a34-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="57a34-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="57a34-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="57a34-124">Authorization</span></span>  | <span data-ttu-id="57a34-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57a34-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57a34-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="57a34-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="57a34-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="57a34-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57a34-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57a34-130">Request body</span></span>
<span data-ttu-id="57a34-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57a34-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57a34-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="57a34-132">Parameter</span></span>    | <span data-ttu-id="57a34-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="57a34-133">Type</span></span>   |<span data-ttu-id="57a34-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="57a34-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57a34-135">opções</span><span class="sxs-lookup"><span data-stu-id="57a34-135">options</span></span>|<span data-ttu-id="57a34-136">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="57a34-136">WorksheetProtectionOptions</span></span>|<span data-ttu-id="57a34-p107">Opcional. Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="57a34-p107">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="57a34-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a34-139">Response</span></span>

<span data-ttu-id="57a34-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57a34-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57a34-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57a34-142">Example</span></span>
<span data-ttu-id="57a34-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="57a34-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57a34-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57a34-144">Request</span></span>
<span data-ttu-id="57a34-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57a34-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="57a34-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a34-146">Response</span></span>
<span data-ttu-id="57a34-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57a34-147">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
