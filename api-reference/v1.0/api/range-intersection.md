---
title: 'Range: Intersection'
description: Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.
author: lumine2008
ms.openlocfilehash: e35bf93a07930b34e984df4a84d5ed30b907ea15
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309685"
---
# <a name="range-intersection"></a><span data-ttu-id="81dbe-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="81dbe-103">Range: Intersection</span></span>

<span data-ttu-id="81dbe-104">Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.</span><span class="sxs-lookup"><span data-stu-id="81dbe-104">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="81dbe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="81dbe-105">Permissions</span></span>
<span data-ttu-id="81dbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81dbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81dbe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81dbe-108">Permission type</span></span>      | <span data-ttu-id="81dbe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81dbe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81dbe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81dbe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81dbe-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81dbe-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="81dbe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81dbe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81dbe-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81dbe-113">Not supported.</span></span>    |
|<span data-ttu-id="81dbe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81dbe-114">Application</span></span> | <span data-ttu-id="81dbe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81dbe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81dbe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81dbe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="81dbe-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81dbe-117">Request headers</span></span>
| <span data-ttu-id="81dbe-118">Nome</span><span class="sxs-lookup"><span data-stu-id="81dbe-118">Name</span></span>       | <span data-ttu-id="81dbe-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="81dbe-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81dbe-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="81dbe-120">Authorization</span></span>  | <span data-ttu-id="81dbe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81dbe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81dbe-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="81dbe-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="81dbe-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="81dbe-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81dbe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81dbe-126">Request body</span></span>
<span data-ttu-id="81dbe-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81dbe-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="81dbe-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="81dbe-128">Parameter</span></span>    | <span data-ttu-id="81dbe-129">Type</span><span class="sxs-lookup"><span data-stu-id="81dbe-129">Type</span></span>   |<span data-ttu-id="81dbe-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="81dbe-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81dbe-131">anotherRange</span><span class="sxs-lookup"><span data-stu-id="81dbe-131">anotherRange</span></span>|<span data-ttu-id="81dbe-132">string</span><span class="sxs-lookup"><span data-stu-id="81dbe-132">string</span></span>|<span data-ttu-id="81dbe-133">O objeto de intervalo ou o endereço do intervalo que será usado para determinar a interseção de intervalos.</span><span class="sxs-lookup"><span data-stu-id="81dbe-133">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="81dbe-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="81dbe-134">Response</span></span>

<span data-ttu-id="81dbe-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81dbe-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81dbe-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81dbe-136">Example</span></span>
<span data-ttu-id="81dbe-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="81dbe-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="81dbe-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81dbe-138">Request</span></span>
<span data-ttu-id="81dbe-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81dbe-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="81dbe-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="81dbe-140">Response</span></span>
<span data-ttu-id="81dbe-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81dbe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->