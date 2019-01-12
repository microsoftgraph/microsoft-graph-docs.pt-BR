---
title: 'RangeFormat: autofitColumns'
description: Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: e5530f0f4ce5f1896b8515c529b5c3bb39a8293b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933698"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="eddb4-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="eddb4-103">RangeFormat: autofitColumns</span></span>

> <span data-ttu-id="eddb4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eddb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eddb4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eddb4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eddb4-106">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="eddb4-106">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="eddb4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eddb4-107">Permissions</span></span>
<span data-ttu-id="eddb4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eddb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eddb4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eddb4-110">Permission type</span></span>      | <span data-ttu-id="eddb4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eddb4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eddb4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eddb4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eddb4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eddb4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eddb4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eddb4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eddb4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eddb4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eddb4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eddb4-116">Application</span></span> | <span data-ttu-id="eddb4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eddb4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eddb4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eddb4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="eddb4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eddb4-119">Request headers</span></span>
| <span data-ttu-id="eddb4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eddb4-120">Name</span></span>       | <span data-ttu-id="eddb4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eddb4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eddb4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eddb4-122">Authorization</span></span>  | <span data-ttu-id="eddb4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eddb4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eddb4-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eddb4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="eddb4-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eddb4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eddb4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eddb4-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="eddb4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eddb4-129">Response</span></span>

<span data-ttu-id="eddb4-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eddb4-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eddb4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eddb4-132">Example</span></span>
<span data-ttu-id="eddb4-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="eddb4-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eddb4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eddb4-134">Request</span></span>
<span data-ttu-id="eddb4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eddb4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitColumns
```

##### <a name="response"></a><span data-ttu-id="eddb4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eddb4-136">Response</span></span>
<span data-ttu-id="eddb4-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eddb4-137">Here is an example of the response.</span></span> 
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
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
