---
title: 'Range: clear'
description: Limpa valores de intervalo, formatação, preenchimento, borda, etc.
ms.openlocfilehash: 2a75530d0a8c366718e7e67f64811e4da9fa27e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034423"
---
# <a name="range-clear"></a><span data-ttu-id="8a238-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="8a238-103">Range: clear</span></span>

> <span data-ttu-id="8a238-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8a238-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a238-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8a238-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a238-106">Limpa valores de intervalo, formatação, preenchimento, borda, etc.</span><span class="sxs-lookup"><span data-stu-id="8a238-106">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="8a238-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a238-107">Permissions</span></span>
<span data-ttu-id="8a238-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a238-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a238-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a238-110">Permission type</span></span>      | <span data-ttu-id="8a238-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a238-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a238-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a238-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a238-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a238-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a238-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a238-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a238-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a238-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a238-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a238-116">Application</span></span> | <span data-ttu-id="8a238-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a238-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a238-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a238-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="8a238-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a238-119">Request headers</span></span>
| <span data-ttu-id="8a238-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8a238-120">Name</span></span>       | <span data-ttu-id="8a238-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a238-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a238-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a238-122">Authorization</span></span>  | <span data-ttu-id="8a238-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a238-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a238-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8a238-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8a238-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8a238-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a238-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a238-128">Request body</span></span>
<span data-ttu-id="8a238-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a238-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8a238-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8a238-130">Parameter</span></span>    | <span data-ttu-id="8a238-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a238-131">Type</span></span>   |<span data-ttu-id="8a238-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a238-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a238-133">applyTo</span><span class="sxs-lookup"><span data-stu-id="8a238-133">applyTo</span></span>|<span data-ttu-id="8a238-134">string</span><span class="sxs-lookup"><span data-stu-id="8a238-134">string</span></span>|<span data-ttu-id="8a238-p105">Opcional. Determina o tipo de ação de limpeza.  Os valores possíveis são: `All`, `Formats` e `Contents`.</span><span class="sxs-lookup"><span data-stu-id="8a238-p105">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="8a238-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a238-138">Response</span></span>

<span data-ttu-id="8a238-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a238-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a238-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a238-141">Example</span></span>
<span data-ttu-id="8a238-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8a238-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a238-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a238-143">Request</span></span>
<span data-ttu-id="8a238-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a238-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="8a238-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a238-145">Response</span></span>
<span data-ttu-id="8a238-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a238-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->