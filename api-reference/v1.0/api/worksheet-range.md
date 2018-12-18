---
title: 'Worksheet: Range'
description: Obtém o objeto de intervalo especificado pelo nome ou endereço.
author: lumine2008
ms.openlocfilehash: fec1ea97be1ca2c094af7e32deac0b6a37f4f086
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319863"
---
# <a name="worksheet-range"></a><span data-ttu-id="3c3ee-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="3c3ee-103">Worksheet: Range</span></span>

<span data-ttu-id="3c3ee-104">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c3ee-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c3ee-105">Permissions</span></span>
<span data-ttu-id="3c3ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c3ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c3ee-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c3ee-108">Permission type</span></span>      | <span data-ttu-id="3c3ee-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c3ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c3ee-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c3ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c3ee-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c3ee-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3c3ee-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c3ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c3ee-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-113">Not supported.</span></span>    |
|<span data-ttu-id="3c3ee-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c3ee-114">Application</span></span> | <span data-ttu-id="3c3ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c3ee-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c3ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="3c3ee-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c3ee-117">Request headers</span></span>
| <span data-ttu-id="3c3ee-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3c3ee-118">Name</span></span>       | <span data-ttu-id="3c3ee-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c3ee-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3c3ee-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c3ee-120">Authorization</span></span>  | <span data-ttu-id="3c3ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c3ee-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3c3ee-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3c3ee-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="3c3ee-126">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3c3ee-126">Function parameters</span></span>

| <span data-ttu-id="3c3ee-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3c3ee-127">Parameter</span></span>    | <span data-ttu-id="3c3ee-128">Type</span><span class="sxs-lookup"><span data-stu-id="3c3ee-128">Type</span></span>   |<span data-ttu-id="3c3ee-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c3ee-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c3ee-130">address</span><span class="sxs-lookup"><span data-stu-id="3c3ee-130">address</span></span>|<span data-ttu-id="3c3ee-131">string</span><span class="sxs-lookup"><span data-stu-id="3c3ee-131">string</span></span>|<span data-ttu-id="3c3ee-p104">Opcional. O endereço ou nome do intervalo. Caso não seja especificado, todo o intervalo da planilha será retornado.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="3c3ee-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c3ee-135">Response</span></span>

<span data-ttu-id="3c3ee-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c3ee-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c3ee-137">Example</span></span>
<span data-ttu-id="3c3ee-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3c3ee-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c3ee-139">Request</span></span>
<span data-ttu-id="3c3ee-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="3c3ee-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c3ee-141">Response</span></span>
<span data-ttu-id="3c3ee-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="3c3ee-145">Se o opcional `address` parâmetro não for especificado, essa função retorna o intervalo de planilha inteira.</span><span class="sxs-lookup"><span data-stu-id="3c3ee-145">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="3c3ee-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c3ee-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="3c3ee-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c3ee-147">Response</span></span>

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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->