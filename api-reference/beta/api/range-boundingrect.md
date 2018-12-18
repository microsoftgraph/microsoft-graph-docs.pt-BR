---
title: 'Range: BoundingRect'
description: .
author: lumine2008
ms.openlocfilehash: 937a6cfa7cbb1d1d95f27139aaa12a8ae444f887
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317294"
---
# <a name="range-boundingrect"></a><span data-ttu-id="3eea0-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="3eea0-103">Range: BoundingRect</span></span>

> <span data-ttu-id="3eea0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3eea0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eea0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3eea0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3eea0-p102">Obtém o menor objeto de intervalo que abrange os intervalos determinados. Por exemplo, GetBoundingRect de "B2:C5" e "D10:E15" é "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="3eea0-p102">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="3eea0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3eea0-108">Permissions</span></span>
<span data-ttu-id="3eea0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eea0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eea0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3eea0-111">Permission type</span></span>      | <span data-ttu-id="3eea0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3eea0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eea0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3eea0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3eea0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3eea0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3eea0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3eea0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eea0-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3eea0-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3eea0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3eea0-117">Application</span></span> | <span data-ttu-id="3eea0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eea0-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3eea0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3eea0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="3eea0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3eea0-120">Request headers</span></span>
| <span data-ttu-id="3eea0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3eea0-121">Name</span></span>       | <span data-ttu-id="3eea0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eea0-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3eea0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3eea0-123">Authorization</span></span>  | <span data-ttu-id="3eea0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3eea0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3eea0-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3eea0-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="3eea0-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3eea0-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eea0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3eea0-129">Request body</span></span>
<span data-ttu-id="3eea0-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3eea0-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3eea0-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3eea0-131">Parameter</span></span>    | <span data-ttu-id="3eea0-132">Type</span><span class="sxs-lookup"><span data-stu-id="3eea0-132">Type</span></span>   |<span data-ttu-id="3eea0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eea0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3eea0-134">anotherRange</span><span class="sxs-lookup"><span data-stu-id="3eea0-134">anotherRange</span></span>|<span data-ttu-id="3eea0-135">string</span><span class="sxs-lookup"><span data-stu-id="3eea0-135">string</span></span>|<span data-ttu-id="3eea0-136">O objeto de intervalo, endereço ou nome do intervalo.</span><span class="sxs-lookup"><span data-stu-id="3eea0-136">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="3eea0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eea0-137">Response</span></span>

<span data-ttu-id="3eea0-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3eea0-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eea0-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3eea0-139">Example</span></span>
<span data-ttu-id="3eea0-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3eea0-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3eea0-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3eea0-141">Request</span></span>
<span data-ttu-id="3eea0-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3eea0-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="3eea0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eea0-143">Response</span></span>
<span data-ttu-id="3eea0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3eea0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->