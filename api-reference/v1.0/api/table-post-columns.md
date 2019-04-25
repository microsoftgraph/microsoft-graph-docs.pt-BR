---
title: Criar TableColumn
description: Use essa API para criar uma nova TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 17c49101decad6ad840ff8c564e204ccd6399072
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520638"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="5b26b-103">Criar TableColumn</span><span class="sxs-lookup"><span data-stu-id="5b26b-103">Create TableColumn</span></span>

<span data-ttu-id="5b26b-104">Use essa API para criar uma nova TableColumn.</span><span class="sxs-lookup"><span data-stu-id="5b26b-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b26b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b26b-105">Permissions</span></span>
<span data-ttu-id="5b26b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b26b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b26b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b26b-108">Permission type</span></span>      | <span data-ttu-id="5b26b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b26b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b26b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b26b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5b26b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b26b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5b26b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b26b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b26b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b26b-113">Not supported.</span></span>    |
|<span data-ttu-id="5b26b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b26b-114">Application</span></span> | <span data-ttu-id="5b26b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b26b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b26b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b26b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="5b26b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b26b-117">Request headers</span></span>
| <span data-ttu-id="5b26b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5b26b-118">Name</span></span>       | <span data-ttu-id="5b26b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b26b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5b26b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b26b-120">Authorization</span></span>  | <span data-ttu-id="5b26b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b26b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b26b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5b26b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5b26b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5b26b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b26b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b26b-126">Request body</span></span>
<span data-ttu-id="5b26b-127">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookTableColumn](../resources/tablecolumn.md) .</span><span class="sxs-lookup"><span data-stu-id="5b26b-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5b26b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b26b-128">Response</span></span>

<span data-ttu-id="5b26b-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [WorkbookTableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b26b-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b26b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b26b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b26b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b26b-131">Request</span></span>
<span data-ttu-id="5b26b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b26b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="5b26b-133">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookTableColumn](../resources/tablecolumn.md) .</span><span class="sxs-lookup"><span data-stu-id="5b26b-133">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5b26b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b26b-134">Response</span></span>
<span data-ttu-id="5b26b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b26b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
