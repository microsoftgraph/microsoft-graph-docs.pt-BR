---
title: Linhas da lista rangeView
description: Recupere uma lista de objetos da exibição de intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9d0d3cb5f29f9588481b5e87c7a20cc96e3850e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522998"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="e8e00-103">Linhas da lista rangeView</span><span class="sxs-lookup"><span data-stu-id="e8e00-103">List rangeView rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8e00-104">Recupere uma lista de objetos da exibição de intervalo.</span><span class="sxs-lookup"><span data-stu-id="e8e00-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8e00-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8e00-105">Permissions</span></span>
<span data-ttu-id="e8e00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8e00-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8e00-108">Permission type</span></span>      | <span data-ttu-id="e8e00-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8e00-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8e00-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8e00-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8e00-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8e00-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8e00-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8e00-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8e00-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8e00-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8e00-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8e00-114">Application</span></span> | <span data-ttu-id="e8e00-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8e00-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8e00-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8e00-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8e00-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8e00-117">Optional query parameters</span></span>
<span data-ttu-id="e8e00-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8e00-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8e00-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e00-119">Request headers</span></span>
| <span data-ttu-id="e8e00-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e8e00-120">Name</span></span>      |<span data-ttu-id="e8e00-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8e00-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8e00-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8e00-122">Authorization</span></span>  | <span data-ttu-id="e8e00-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8e00-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8e00-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e8e00-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e8e00-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e8e00-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8e00-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e00-128">Request body</span></span>
<span data-ttu-id="e8e00-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8e00-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8e00-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e00-130">Response</span></span>

<span data-ttu-id="e8e00-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8e00-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8e00-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8e00-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8e00-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e00-133">Request</span></span>
<span data-ttu-id="e8e00-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8e00-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/rows 
```
##### <a name="response"></a><span data-ttu-id="e8e00-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e00-135">Response</span></span>
<span data-ttu-id="e8e00-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8e00-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrangeview-list-rows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
