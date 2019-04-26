---
title: Criar RangeBorder
description: Use essa API para criar uma nova RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f9a69b7fc8a8d5e81c67847849cab30b8391caa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331691"
---
# <a name="create-rangeborder"></a><span data-ttu-id="40ffe-103">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="40ffe-103">Create RangeBorder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40ffe-104">Use essa API para criar uma nova RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="40ffe-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="40ffe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="40ffe-105">Permissions</span></span>
<span data-ttu-id="40ffe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40ffe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ffe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40ffe-108">Permission type</span></span>      | <span data-ttu-id="40ffe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40ffe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40ffe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40ffe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40ffe-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40ffe-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="40ffe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40ffe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40ffe-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40ffe-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="40ffe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40ffe-114">Application</span></span> | <span data-ttu-id="40ffe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40ffe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40ffe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40ffe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="40ffe-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40ffe-117">Request headers</span></span>
| <span data-ttu-id="40ffe-118">Nome</span><span class="sxs-lookup"><span data-stu-id="40ffe-118">Name</span></span>       | <span data-ttu-id="40ffe-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="40ffe-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="40ffe-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="40ffe-120">Authorization</span></span>  | <span data-ttu-id="40ffe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40ffe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40ffe-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="40ffe-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="40ffe-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="40ffe-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40ffe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40ffe-126">Request body</span></span>
<span data-ttu-id="40ffe-127">No corpo da solicitação, forneça uma representação JSON do objeto [workbookRangeBorder](../resources/workbookrangeborder.md) .</span><span class="sxs-lookup"><span data-stu-id="40ffe-127">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="40ffe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="40ffe-128">Response</span></span>

<span data-ttu-id="40ffe-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [workbookRangeBorder](../resources/workbookrangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40ffe-129">If successful, this method returns `201 Created` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40ffe-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40ffe-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40ffe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40ffe-131">Request</span></span>
<span data-ttu-id="40ffe-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40ffe-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="40ffe-133">No corpo da solicitação, forneça uma representação JSON do objeto [workbookRangeBorder](../resources/workbookrangeborder.md) .</span><span class="sxs-lookup"><span data-stu-id="40ffe-133">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="40ffe-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="40ffe-134">Response</span></span>
<span data-ttu-id="40ffe-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40ffe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
