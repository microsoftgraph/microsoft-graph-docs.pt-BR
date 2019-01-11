---
title: Obter WorksheetProtection
description: Leia as propriedades e os relacionamentos do objeto worksheetprotection.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d18b20b9d4af7dc9351c90039290cf93d2aec741
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853939"
---
# <a name="get-worksheetprotection"></a><span data-ttu-id="f7f17-103">Obter WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="f7f17-103">Get WorksheetProtection</span></span>

<span data-ttu-id="f7f17-104">Leia as propriedades e os relacionamentos do objeto worksheetprotection.</span><span class="sxs-lookup"><span data-stu-id="f7f17-104">Retrieve the properties and relationships of worksheetprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7f17-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7f17-105">Permissions</span></span>
<span data-ttu-id="f7f17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7f17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7f17-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7f17-108">Permission type</span></span>      | <span data-ttu-id="f7f17-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7f17-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7f17-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7f17-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7f17-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7f17-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7f17-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7f17-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7f17-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7f17-113">Not supported.</span></span>    |
|<span data-ttu-id="f7f17-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7f17-114">Application</span></span> | <span data-ttu-id="f7f17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7f17-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7f17-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7f17-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7f17-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f7f17-117">Optional query parameters</span></span>
<span data-ttu-id="f7f17-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f7f17-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7f17-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7f17-119">Request headers</span></span>
| <span data-ttu-id="f7f17-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f7f17-120">Name</span></span>      |<span data-ttu-id="f7f17-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7f17-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7f17-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7f17-122">Authorization</span></span>  | <span data-ttu-id="f7f17-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7f17-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7f17-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f7f17-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f7f17-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f7f17-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7f17-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7f17-128">Request body</span></span>
<span data-ttu-id="f7f17-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7f17-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7f17-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7f17-130">Response</span></span>

<span data-ttu-id="f7f17-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [WorkbookWorksheetProtection](../resources/worksheetprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7f17-131">If successful, this method returns a `200 OK` response code and [WorkbookWorksheetProtection](../resources/worksheetprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7f17-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7f17-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7f17-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7f17-133">Request</span></span>
<span data-ttu-id="f7f17-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7f17-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheetprotection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection
```
##### <a name="response"></a><span data-ttu-id="f7f17-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7f17-135">Response</span></span>
<span data-ttu-id="f7f17-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7f17-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 23

{
  "protected": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get WorksheetProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
