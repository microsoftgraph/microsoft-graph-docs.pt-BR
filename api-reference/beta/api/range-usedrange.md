---
title: 'Range: UsedRange'
description: Retorna o intervalo usado do objeto range determinado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0ae8f8bec1eea6f2e13b4c4248d55afbb28cf19d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928063"
---
# <a name="range-usedrange"></a><span data-ttu-id="a2bbf-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="a2bbf-103">Range: UsedRange</span></span>

> <span data-ttu-id="a2bbf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2bbf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2bbf-106">Retorna o intervalo usado do objeto range determinado.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-106">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2bbf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2bbf-107">Permissions</span></span>
<span data-ttu-id="a2bbf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2bbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2bbf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2bbf-110">Permission type</span></span>      | <span data-ttu-id="a2bbf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2bbf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2bbf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2bbf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a2bbf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2bbf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a2bbf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2bbf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2bbf-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2bbf-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a2bbf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2bbf-116">Application</span></span> | <span data-ttu-id="a2bbf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2bbf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2bbf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="a2bbf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bbf-119">Request headers</span></span>
| <span data-ttu-id="a2bbf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a2bbf-120">Name</span></span>       | <span data-ttu-id="a2bbf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2bbf-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a2bbf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2bbf-122">Authorization</span></span>  | <span data-ttu-id="a2bbf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2bbf-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a2bbf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a2bbf-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2bbf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bbf-128">Request body</span></span>
<span data-ttu-id="a2bbf-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a2bbf-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a2bbf-130">Parameter</span></span>    | <span data-ttu-id="a2bbf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2bbf-131">Type</span></span>   |<span data-ttu-id="a2bbf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2bbf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2bbf-133">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="a2bbf-133">valuesOnly</span></span>|<span data-ttu-id="a2bbf-134">booliano</span><span class="sxs-lookup"><span data-stu-id="a2bbf-134">boolean</span></span>|<span data-ttu-id="a2bbf-p105">Opcional. Considera apenas as células com valores como células usadas.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-p105">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="a2bbf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2bbf-137">Response</span></span>

<span data-ttu-id="a2bbf-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2bbf-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2bbf-139">Example</span></span>
<span data-ttu-id="a2bbf-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a2bbf-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bbf-141">Request</span></span>
<span data-ttu-id="a2bbf-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="a2bbf-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2bbf-143">Response</span></span>
<span data-ttu-id="a2bbf-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2bbf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
