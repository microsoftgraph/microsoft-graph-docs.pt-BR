---
title: Obter gráfico
description: Recupera as propriedades e os relacionamentos do objeto de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7d81312cac63f17a69ec9076287209a67c0a1f23
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580803"
---
# <a name="get-chart"></a><span data-ttu-id="803fd-103">Obter gráfico</span><span class="sxs-lookup"><span data-stu-id="803fd-103">Get Chart</span></span>

<span data-ttu-id="803fd-104">Recupera as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="803fd-104">Retrieve the properties and relationships of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="803fd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="803fd-105">Permissions</span></span>
<span data-ttu-id="803fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="803fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="803fd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="803fd-108">Permission type</span></span>      | <span data-ttu-id="803fd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="803fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="803fd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="803fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="803fd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="803fd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="803fd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="803fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="803fd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="803fd-113">Not supported.</span></span>    |
|<span data-ttu-id="803fd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="803fd-114">Application</span></span> | <span data-ttu-id="803fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="803fd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="803fd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="803fd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="803fd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="803fd-117">Optional query parameters</span></span>
<span data-ttu-id="803fd-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="803fd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="803fd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="803fd-119">Request headers</span></span>
| <span data-ttu-id="803fd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="803fd-120">Name</span></span>      |<span data-ttu-id="803fd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="803fd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="803fd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="803fd-122">Authorization</span></span>  | <span data-ttu-id="803fd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="803fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="803fd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="803fd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="803fd-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="803fd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="803fd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="803fd-128">Request body</span></span>
<span data-ttu-id="803fd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="803fd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="803fd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="803fd-130">Response</span></span>

<span data-ttu-id="803fd-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="803fd-131">If successful, this method returns a `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="803fd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="803fd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="803fd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="803fd-133">Request</span></span>
<span data-ttu-id="803fd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="803fd-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chart"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
```
##### <a name="response"></a><span data-ttu-id="803fd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="803fd-135">Response</span></span>
<span data-ttu-id="803fd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="803fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
