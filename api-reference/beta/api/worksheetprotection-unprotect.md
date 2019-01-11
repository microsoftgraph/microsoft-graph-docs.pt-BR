---
title: 'WorksheetProtection: unprotect'
description: Desprotege uma planilha.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 52feaf77964949fee9bbedbf3ced2967226bb486
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850516"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="f14cf-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="f14cf-103">WorksheetProtection: unprotect</span></span>

> <span data-ttu-id="f14cf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f14cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f14cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f14cf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f14cf-106">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="f14cf-106">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="f14cf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f14cf-107">Permissions</span></span>
<span data-ttu-id="f14cf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f14cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f14cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f14cf-110">Permission type</span></span>      | <span data-ttu-id="f14cf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f14cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f14cf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f14cf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f14cf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f14cf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f14cf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f14cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f14cf-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f14cf-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f14cf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f14cf-116">Application</span></span> | <span data-ttu-id="f14cf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f14cf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f14cf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f14cf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="f14cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f14cf-119">Request headers</span></span>
| <span data-ttu-id="f14cf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f14cf-120">Name</span></span>       | <span data-ttu-id="f14cf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f14cf-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f14cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f14cf-122">Authorization</span></span>  | <span data-ttu-id="f14cf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f14cf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f14cf-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f14cf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f14cf-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f14cf-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f14cf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f14cf-128">Request body</span></span>
<span data-ttu-id="f14cf-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f14cf-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f14cf-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f14cf-130">Parameter</span></span>    | <span data-ttu-id="f14cf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f14cf-131">Type</span></span>   |<span data-ttu-id="f14cf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f14cf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f14cf-133">password</span><span class="sxs-lookup"><span data-stu-id="f14cf-133">password</span></span>|<span data-ttu-id="f14cf-134">string</span><span class="sxs-lookup"><span data-stu-id="f14cf-134">string</span></span>|<span data-ttu-id="f14cf-p105">Opcional. Senha de proteção para a planilha.</span><span class="sxs-lookup"><span data-stu-id="f14cf-p105">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="f14cf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f14cf-137">Response</span></span>

<span data-ttu-id="f14cf-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f14cf-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f14cf-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f14cf-140">Example</span></span>
<span data-ttu-id="f14cf-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f14cf-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f14cf-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f14cf-142">Request</span></span>
<span data-ttu-id="f14cf-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f14cf-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="f14cf-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f14cf-144">Response</span></span>
<span data-ttu-id="f14cf-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f14cf-145">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
