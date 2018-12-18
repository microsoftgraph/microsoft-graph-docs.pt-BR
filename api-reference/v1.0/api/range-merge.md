---
title: 'Range: merge'
description: Mescla as células do intervalo em uma região da planilha.
author: lumine2008
ms.openlocfilehash: 87fc6fab83f1f03d40a1363277bfec511839bad6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312772"
---
# <a name="range-merge"></a><span data-ttu-id="8e748-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="8e748-103">Range: merge</span></span>

<span data-ttu-id="8e748-104">Mescla as células do intervalo em uma região da planilha.</span><span class="sxs-lookup"><span data-stu-id="8e748-104">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="8e748-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e748-105">Permissions</span></span>
<span data-ttu-id="8e748-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e748-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e748-108">Permission type</span></span>      | <span data-ttu-id="8e748-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e748-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e748-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e748-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8e748-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e748-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8e748-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e748-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e748-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e748-113">Not supported.</span></span>    |
|<span data-ttu-id="8e748-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e748-114">Application</span></span> | <span data-ttu-id="8e748-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e748-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e748-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e748-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="8e748-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e748-117">Request headers</span></span>
| <span data-ttu-id="8e748-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8e748-118">Name</span></span>       | <span data-ttu-id="8e748-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e748-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8e748-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e748-120">Authorization</span></span>  | <span data-ttu-id="8e748-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e748-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e748-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8e748-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8e748-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8e748-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e748-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e748-126">Request body</span></span>
<span data-ttu-id="8e748-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e748-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e748-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8e748-128">Parameter</span></span>    | <span data-ttu-id="8e748-129">Type</span><span class="sxs-lookup"><span data-stu-id="8e748-129">Type</span></span>   |<span data-ttu-id="8e748-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e748-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e748-131">across</span><span class="sxs-lookup"><span data-stu-id="8e748-131">across</span></span>|<span data-ttu-id="8e748-132">booliano</span><span class="sxs-lookup"><span data-stu-id="8e748-132">boolean</span></span>|<span data-ttu-id="8e748-p104">Opcional. Defina true para mesclar células em todas as linhas do intervalo especificado como células mescladas separadamente. O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="8e748-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="8e748-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e748-136">Response</span></span>

<span data-ttu-id="8e748-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e748-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e748-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e748-139">Example</span></span>
<span data-ttu-id="8e748-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8e748-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8e748-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e748-141">Request</span></span>
<span data-ttu-id="8e748-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e748-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="8e748-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e748-143">Response</span></span>
<span data-ttu-id="8e748-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e748-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->