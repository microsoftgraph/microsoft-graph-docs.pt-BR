---
title: 'WorksheetProtection: unprotect'
description: Desprotege uma planilha.
ms.openlocfilehash: 32909d81119c326172a12d346ea53d9f8eb2b71b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039663"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="c797b-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="c797b-103">WorksheetProtection: unprotect</span></span>

> <span data-ttu-id="c797b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c797b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c797b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c797b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c797b-106">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="c797b-106">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="c797b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c797b-107">Permissions</span></span>
<span data-ttu-id="c797b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c797b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c797b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c797b-110">Permission type</span></span>      | <span data-ttu-id="c797b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c797b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c797b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c797b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c797b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c797b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c797b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c797b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c797b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c797b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c797b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c797b-116">Application</span></span> | <span data-ttu-id="c797b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c797b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c797b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c797b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="c797b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c797b-119">Request headers</span></span>
| <span data-ttu-id="c797b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c797b-120">Name</span></span>       | <span data-ttu-id="c797b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c797b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c797b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c797b-122">Authorization</span></span>  | <span data-ttu-id="c797b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c797b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c797b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c797b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c797b-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c797b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c797b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c797b-128">Request body</span></span>
<span data-ttu-id="c797b-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c797b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c797b-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c797b-130">Parameter</span></span>    | <span data-ttu-id="c797b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c797b-131">Type</span></span>   |<span data-ttu-id="c797b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c797b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c797b-133">password</span><span class="sxs-lookup"><span data-stu-id="c797b-133">password</span></span>|<span data-ttu-id="c797b-134">string</span><span class="sxs-lookup"><span data-stu-id="c797b-134">string</span></span>|<span data-ttu-id="c797b-p105">Opcional. Senha de proteção para a planilha.</span><span class="sxs-lookup"><span data-stu-id="c797b-p105">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="c797b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c797b-137">Response</span></span>

<span data-ttu-id="c797b-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c797b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c797b-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c797b-140">Example</span></span>
<span data-ttu-id="c797b-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c797b-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c797b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c797b-142">Request</span></span>
<span data-ttu-id="c797b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c797b-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c797b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c797b-144">Response</span></span>
<span data-ttu-id="c797b-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c797b-145">Here is an example of the response.</span></span> 
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