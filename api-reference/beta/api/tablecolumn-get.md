---
title: Obter TableColumn
description: Recupere as propriedades e os relacionamentos do objeto tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 19f5620cd2a632de837f941d1ac9ccb1c523f5a9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330364"
---
# <a name="get-tablecolumn"></a><span data-ttu-id="9380c-103">Obter TableColumn</span><span class="sxs-lookup"><span data-stu-id="9380c-103">Get TableColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9380c-104">Recupere as propriedades e os relacionamentos do objeto tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="9380c-104">Retrieve the properties and relationships of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9380c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9380c-105">Permissions</span></span>
<span data-ttu-id="9380c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9380c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9380c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9380c-108">Permission type</span></span>      | <span data-ttu-id="9380c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9380c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9380c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9380c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9380c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9380c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9380c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9380c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9380c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9380c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9380c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9380c-114">Application</span></span> | <span data-ttu-id="9380c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9380c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9380c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9380c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9380c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9380c-117">Optional query parameters</span></span>
<span data-ttu-id="9380c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9380c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9380c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9380c-119">Request headers</span></span>
| <span data-ttu-id="9380c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9380c-120">Name</span></span>      |<span data-ttu-id="9380c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9380c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9380c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9380c-122">Authorization</span></span>  | <span data-ttu-id="9380c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9380c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9380c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9380c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9380c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9380c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9380c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9380c-128">Request body</span></span>
<span data-ttu-id="9380c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9380c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9380c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9380c-130">Response</span></span>

<span data-ttu-id="9380c-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9380c-131">If successful, this method returns a `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9380c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9380c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9380c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9380c-133">Request</span></span>
<span data-ttu-id="9380c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9380c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
```
##### <a name="response"></a><span data-ttu-id="9380c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9380c-135">Response</span></span>
<span data-ttu-id="9380c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9380c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
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
<!--
{
  "type": "#page.annotation",
  "description": "Get TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
