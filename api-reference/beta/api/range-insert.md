---
title: 'Range: insert'
description: Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.
localization_priority: Normal
ms.openlocfilehash: 0e7ab0d729dad4eec7fb455774cfed19bf4f5013
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831511"
---
# <a name="range-insert"></a><span data-ttu-id="11503-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="11503-104">Range: insert</span></span>

> <span data-ttu-id="11503-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11503-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11503-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11503-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11503-p103">Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.</span><span class="sxs-lookup"><span data-stu-id="11503-p103">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="11503-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="11503-109">Permissions</span></span>
<span data-ttu-id="11503-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11503-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11503-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11503-112">Permission type</span></span>      | <span data-ttu-id="11503-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11503-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11503-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11503-114">Delegated (work or school account)</span></span> | <span data-ttu-id="11503-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11503-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11503-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11503-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11503-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11503-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11503-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11503-118">Application</span></span> | <span data-ttu-id="11503-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11503-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11503-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11503-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="11503-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11503-121">Request headers</span></span>
| <span data-ttu-id="11503-122">Nome</span><span class="sxs-lookup"><span data-stu-id="11503-122">Name</span></span>       | <span data-ttu-id="11503-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="11503-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11503-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="11503-124">Authorization</span></span>  | <span data-ttu-id="11503-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11503-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11503-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="11503-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="11503-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="11503-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11503-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11503-130">Request body</span></span>
<span data-ttu-id="11503-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11503-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11503-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="11503-132">Parameter</span></span>    | <span data-ttu-id="11503-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="11503-133">Type</span></span>   |<span data-ttu-id="11503-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="11503-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11503-135">shift</span><span class="sxs-lookup"><span data-stu-id="11503-135">shift</span></span>|<span data-ttu-id="11503-136">string</span><span class="sxs-lookup"><span data-stu-id="11503-136">string</span></span>|<span data-ttu-id="11503-p107">Especifica como deslocar as células.  Os valores possíveis são: `Down` e `Right`.</span><span class="sxs-lookup"><span data-stu-id="11503-p107">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="11503-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="11503-139">Response</span></span>

<span data-ttu-id="11503-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11503-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11503-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11503-141">Example</span></span>
<span data-ttu-id="11503-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="11503-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="11503-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11503-143">Request</span></span>
<span data-ttu-id="11503-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11503-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="11503-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="11503-145">Response</span></span>
<span data-ttu-id="11503-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11503-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
