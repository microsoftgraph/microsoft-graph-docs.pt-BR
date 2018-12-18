---
title: 'Range: delete'
description: Exclui as células associadas ao intervalo.
author: lumine2008
ms.openlocfilehash: 00b6d8a35012a3e6d1e6c0755a077d0575baa00e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352700"
---
# <a name="range-delete"></a><span data-ttu-id="7b600-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="7b600-103">Range: delete</span></span>

> <span data-ttu-id="7b600-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7b600-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b600-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7b600-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b600-106">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="7b600-106">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="7b600-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b600-107">Permissions</span></span>
<span data-ttu-id="7b600-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b600-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b600-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b600-110">Permission type</span></span>      | <span data-ttu-id="7b600-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b600-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b600-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b600-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7b600-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b600-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7b600-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b600-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b600-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b600-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7b600-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b600-116">Application</span></span> | <span data-ttu-id="7b600-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b600-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b600-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b600-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="7b600-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b600-119">Request headers</span></span>
| <span data-ttu-id="7b600-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7b600-120">Name</span></span>       | <span data-ttu-id="7b600-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b600-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7b600-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b600-122">Authorization</span></span>  | <span data-ttu-id="7b600-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b600-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b600-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7b600-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7b600-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7b600-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b600-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b600-128">Request body</span></span>
<span data-ttu-id="7b600-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b600-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7b600-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7b600-130">Parameter</span></span>    | <span data-ttu-id="7b600-131">Type</span><span class="sxs-lookup"><span data-stu-id="7b600-131">Type</span></span>   |<span data-ttu-id="7b600-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b600-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b600-133">shift</span><span class="sxs-lookup"><span data-stu-id="7b600-133">shift</span></span>|<span data-ttu-id="7b600-134">string</span><span class="sxs-lookup"><span data-stu-id="7b600-134">string</span></span>|<span data-ttu-id="7b600-p105">Especifica como deslocar as células.  Os valores possíveis são: `Up` e `Left`.</span><span class="sxs-lookup"><span data-stu-id="7b600-p105">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="7b600-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b600-137">Response</span></span>

<span data-ttu-id="7b600-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b600-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b600-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b600-140">Example</span></span>
<span data-ttu-id="7b600-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7b600-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7b600-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b600-142">Request</span></span>
<span data-ttu-id="7b600-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b600-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="7b600-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b600-144">Response</span></span>
<span data-ttu-id="7b600-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b600-145">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->