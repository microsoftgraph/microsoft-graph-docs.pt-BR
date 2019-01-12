---
title: Criar TableColumn
description: Use essa API para criar uma nova TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c6a0dc30be0e423129a0bd7ec9c6582e6f582d96
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959780"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="9f8a8-103">Criar TableColumn</span><span class="sxs-lookup"><span data-stu-id="9f8a8-103">Create TableColumn</span></span>

> <span data-ttu-id="9f8a8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9f8a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f8a8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9f8a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f8a8-106">Use essa API para criar uma nova TableColumn.</span><span class="sxs-lookup"><span data-stu-id="9f8a8-106">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f8a8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f8a8-107">Permissions</span></span>
<span data-ttu-id="9f8a8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f8a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f8a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f8a8-110">Permission type</span></span>      | <span data-ttu-id="9f8a8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f8a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f8a8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f8a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9f8a8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f8a8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f8a8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f8a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f8a8-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f8a8-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f8a8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f8a8-116">Application</span></span> | <span data-ttu-id="9f8a8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f8a8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f8a8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f8a8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="9f8a8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f8a8-119">Request headers</span></span>
| <span data-ttu-id="9f8a8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9f8a8-120">Name</span></span>       | <span data-ttu-id="9f8a8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f8a8-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9f8a8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f8a8-122">Authorization</span></span>  | <span data-ttu-id="9f8a8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f8a8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f8a8-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9f8a8-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9f8a8-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9f8a8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f8a8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f8a8-128">Request body</span></span>
<span data-ttu-id="9f8a8-129">No corpo da solicitação, forneça uma representação JSON do objeto [TableColum](../resources/tablecolumn.md).</span><span class="sxs-lookup"><span data-stu-id="9f8a8-129">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9f8a8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f8a8-130">Response</span></span>

<span data-ttu-id="9f8a8-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [TableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f8a8-131">If successful, this method returns `201 Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f8a8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f8a8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f8a8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f8a8-133">Request</span></span>
<span data-ttu-id="9f8a8-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f8a8-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="9f8a8-135">No corpo da solicitação, forneça uma representação JSON do objeto [TableColum](../resources/tablecolumn.md).</span><span class="sxs-lookup"><span data-stu-id="9f8a8-135">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9f8a8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f8a8-136">Response</span></span>
<span data-ttu-id="9f8a8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f8a8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
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
