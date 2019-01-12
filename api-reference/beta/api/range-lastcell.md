---
title: 'Range: LastCell'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 56fd2adea1f2f3bd13e85b035f81835cd18ea0f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966325"
---
# <a name="range-lastcell"></a><span data-ttu-id="52a5a-103">Range: LastCell</span><span class="sxs-lookup"><span data-stu-id="52a5a-103">Range: LastCell</span></span>

> <span data-ttu-id="52a5a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="52a5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52a5a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="52a5a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52a5a-p102">Obtém a última célula do intervalo. Por exemplo, a última célula de "B2:D5" é "D5".</span><span class="sxs-lookup"><span data-stu-id="52a5a-p102">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="52a5a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="52a5a-108">Permissions</span></span>
<span data-ttu-id="52a5a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52a5a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52a5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52a5a-111">Permission type</span></span>      | <span data-ttu-id="52a5a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52a5a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52a5a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52a5a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="52a5a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52a5a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52a5a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52a5a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52a5a-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52a5a-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52a5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52a5a-117">Application</span></span> | <span data-ttu-id="52a5a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52a5a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52a5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52a5a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastCell
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastCell
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastCell

```
## <a name="request-headers"></a><span data-ttu-id="52a5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52a5a-120">Request headers</span></span>
| <span data-ttu-id="52a5a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="52a5a-121">Name</span></span>       | <span data-ttu-id="52a5a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="52a5a-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="52a5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52a5a-123">Authorization</span></span>  | <span data-ttu-id="52a5a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52a5a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52a5a-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="52a5a-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="52a5a-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="52a5a-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52a5a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52a5a-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="52a5a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="52a5a-130">Response</span></span>

<span data-ttu-id="52a5a-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52a5a-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52a5a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52a5a-132">Example</span></span>
<span data-ttu-id="52a5a-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="52a5a-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="52a5a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52a5a-134">Request</span></span>
<span data-ttu-id="52a5a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52a5a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastcell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastCell
```

##### <a name="response"></a><span data-ttu-id="52a5a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="52a5a-136">Response</span></span>
<span data-ttu-id="52a5a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52a5a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastCell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
