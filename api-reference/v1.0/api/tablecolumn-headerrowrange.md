---
title: 'TableColumn: HeaderRowRange'
description: Obtém o objeto de intervalo associado à linha de cabeçalho da coluna.
ms.openlocfilehash: 2de261d3e5fdea039ed081d1763cdc6d71f187ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006930"
---
# <a name="tablecolumn-headerrowrange"></a><span data-ttu-id="46d45-103">TableColumn: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="46d45-103">TableColumn: HeaderRowRange</span></span>

<span data-ttu-id="46d45-104">Obtém o objeto de intervalo associado à linha de cabeçalho da coluna.</span><span class="sxs-lookup"><span data-stu-id="46d45-104">Gets the range object associated with the header row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="46d45-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="46d45-105">Permissions</span></span>
<span data-ttu-id="46d45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46d45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46d45-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46d45-108">Permission type</span></span>      | <span data-ttu-id="46d45-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46d45-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46d45-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46d45-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46d45-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46d45-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46d45-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46d45-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46d45-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46d45-113">Not supported.</span></span>    |
|<span data-ttu-id="46d45-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46d45-114">Application</span></span> | <span data-ttu-id="46d45-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46d45-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46d45-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46d45-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/headerRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="46d45-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46d45-117">Request headers</span></span>
| <span data-ttu-id="46d45-118">Nome</span><span class="sxs-lookup"><span data-stu-id="46d45-118">Name</span></span>       | <span data-ttu-id="46d45-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="46d45-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46d45-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="46d45-120">Authorization</span></span>  | <span data-ttu-id="46d45-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46d45-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46d45-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="46d45-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="46d45-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="46d45-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d45-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46d45-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="46d45-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="46d45-127">Response</span></span>

<span data-ttu-id="46d45-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46d45-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46d45-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46d45-129">Example</span></span>
<span data-ttu-id="46d45-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="46d45-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="46d45-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46d45-131">Request</span></span>
<span data-ttu-id="46d45-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46d45-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_headerrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/headerRowRange
```

##### <a name="response"></a><span data-ttu-id="46d45-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="46d45-133">Response</span></span>
<span data-ttu-id="46d45-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46d45-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
  "description": "TableColumn: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->