---
title: 'Range: LastCell'
description: .
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 38d92e885d56b28b98d5a2720d7198fccd0b8a5e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889223"
---
# <a name="range-lastcell"></a><span data-ttu-id="6c97b-103">Range: LastCell</span><span class="sxs-lookup"><span data-stu-id="6c97b-103">Range: LastCell</span></span>

> <span data-ttu-id="6c97b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c97b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c97b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c97b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c97b-p102">Obtém a última célula do intervalo. Por exemplo, a última célula de "B2:D5" é "D5".</span><span class="sxs-lookup"><span data-stu-id="6c97b-p102">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="6c97b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c97b-108">Permissions</span></span>
<span data-ttu-id="6c97b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c97b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c97b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c97b-111">Permission type</span></span>      | <span data-ttu-id="6c97b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c97b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c97b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c97b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6c97b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c97b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c97b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c97b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c97b-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c97b-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c97b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c97b-117">Application</span></span> | <span data-ttu-id="6c97b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c97b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c97b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c97b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastCell
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastCell
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastCell

```
## <a name="request-headers"></a><span data-ttu-id="6c97b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c97b-120">Request headers</span></span>
| <span data-ttu-id="6c97b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6c97b-121">Name</span></span>       | <span data-ttu-id="6c97b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c97b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6c97b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c97b-123">Authorization</span></span>  | <span data-ttu-id="6c97b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c97b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c97b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6c97b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="6c97b-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6c97b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c97b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c97b-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6c97b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c97b-130">Response</span></span>

<span data-ttu-id="6c97b-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c97b-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c97b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c97b-132">Example</span></span>
<span data-ttu-id="6c97b-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6c97b-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6c97b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c97b-134">Request</span></span>
<span data-ttu-id="6c97b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c97b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastcell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastCell
```

##### <a name="response"></a><span data-ttu-id="6c97b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c97b-136">Response</span></span>
<span data-ttu-id="6c97b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c97b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
