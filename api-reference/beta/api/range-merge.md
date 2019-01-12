---
title: 'Range: merge'
description: Mescla as células do intervalo em uma região da planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 151163604bc7eada167daebdb325857cc6e87ce4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990520"
---
# <a name="range-merge"></a><span data-ttu-id="c9333-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="c9333-103">Range: merge</span></span>

> <span data-ttu-id="c9333-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9333-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9333-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9333-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9333-106">Mescla as células do intervalo em uma região da planilha.</span><span class="sxs-lookup"><span data-stu-id="c9333-106">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9333-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9333-107">Permissions</span></span>
<span data-ttu-id="c9333-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9333-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9333-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9333-110">Permission type</span></span>      | <span data-ttu-id="c9333-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9333-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9333-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9333-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c9333-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9333-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c9333-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9333-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9333-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9333-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c9333-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9333-116">Application</span></span> | <span data-ttu-id="c9333-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9333-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9333-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9333-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="c9333-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9333-119">Request headers</span></span>
| <span data-ttu-id="c9333-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c9333-120">Name</span></span>       | <span data-ttu-id="c9333-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9333-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c9333-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9333-122">Authorization</span></span>  | <span data-ttu-id="c9333-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9333-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9333-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c9333-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c9333-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c9333-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9333-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9333-128">Request body</span></span>
<span data-ttu-id="c9333-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9333-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9333-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c9333-130">Parameter</span></span>    | <span data-ttu-id="c9333-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9333-131">Type</span></span>   |<span data-ttu-id="c9333-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9333-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9333-133">across</span><span class="sxs-lookup"><span data-stu-id="c9333-133">across</span></span>|<span data-ttu-id="c9333-134">booliano</span><span class="sxs-lookup"><span data-stu-id="c9333-134">boolean</span></span>|<span data-ttu-id="c9333-p105">Opcional. Defina true para mesclar células em todas as linhas do intervalo especificado como células mescladas separadamente. O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="c9333-p105">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="c9333-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9333-138">Response</span></span>

<span data-ttu-id="c9333-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9333-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9333-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9333-141">Example</span></span>
<span data-ttu-id="c9333-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c9333-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c9333-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9333-143">Request</span></span>
<span data-ttu-id="c9333-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9333-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="c9333-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9333-145">Response</span></span>
<span data-ttu-id="c9333-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9333-146">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
