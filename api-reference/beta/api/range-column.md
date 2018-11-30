---
title: 'Range: Column'
description: Obtém uma coluna incluída no intervalo.
ms.openlocfilehash: dde991dff164f5abab34c0acccc4127ece76b673
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038710"
---
# <a name="range-column"></a><span data-ttu-id="16f5d-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="16f5d-103">Range: Column</span></span>

> <span data-ttu-id="16f5d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16f5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16f5d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16f5d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16f5d-106">Obtém uma coluna incluída no intervalo.</span><span class="sxs-lookup"><span data-stu-id="16f5d-106">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="16f5d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16f5d-107">Permissions</span></span>
<span data-ttu-id="16f5d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16f5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16f5d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16f5d-110">Permission type</span></span>      | <span data-ttu-id="16f5d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16f5d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16f5d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16f5d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16f5d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16f5d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16f5d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16f5d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16f5d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16f5d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16f5d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16f5d-116">Application</span></span> | <span data-ttu-id="16f5d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16f5d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16f5d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16f5d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Column
GET /workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="16f5d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16f5d-119">Request headers</span></span>
| <span data-ttu-id="16f5d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="16f5d-120">Name</span></span>       | <span data-ttu-id="16f5d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="16f5d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="16f5d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16f5d-122">Authorization</span></span>  | <span data-ttu-id="16f5d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16f5d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16f5d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="16f5d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="16f5d-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="16f5d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16f5d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16f5d-128">Request body</span></span>
<span data-ttu-id="16f5d-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16f5d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="16f5d-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="16f5d-130">Parameter</span></span>    | <span data-ttu-id="16f5d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="16f5d-131">Type</span></span>   |<span data-ttu-id="16f5d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="16f5d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16f5d-133">column</span><span class="sxs-lookup"><span data-stu-id="16f5d-133">column</span></span>|<span data-ttu-id="16f5d-134">número</span><span class="sxs-lookup"><span data-stu-id="16f5d-134">number</span></span>|<span data-ttu-id="16f5d-p105">O número da coluna do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="16f5d-p105">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="16f5d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="16f5d-137">Response</span></span>

<span data-ttu-id="16f5d-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16f5d-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16f5d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16f5d-139">Example</span></span>
<span data-ttu-id="16f5d-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="16f5d-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="16f5d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16f5d-141">Request</span></span>
<span data-ttu-id="16f5d-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16f5d-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Column
Content-type: application/json
Content-length: 21

{
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="16f5d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="16f5d-143">Response</span></span>
<span data-ttu-id="16f5d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16f5d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->