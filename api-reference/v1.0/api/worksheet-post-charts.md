---
title: Criar gráfico
description: Use esta API para criar um novo gráfico.
ms.openlocfilehash: 95ca5233ef21ee73b244720493d07913fec9d088
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004587"
---
# <a name="create-chart"></a><span data-ttu-id="fea1f-103">Criar gráfico</span><span class="sxs-lookup"><span data-stu-id="fea1f-103">Create Chart</span></span>

<span data-ttu-id="fea1f-104">Use esta API para criar um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="fea1f-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="fea1f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fea1f-105">Permissions</span></span>
<span data-ttu-id="fea1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fea1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fea1f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fea1f-108">Permission type</span></span>      | <span data-ttu-id="fea1f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fea1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fea1f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fea1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fea1f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fea1f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fea1f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fea1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fea1f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fea1f-113">Not supported.</span></span>    |
|<span data-ttu-id="fea1f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fea1f-114">Application</span></span> | <span data-ttu-id="fea1f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fea1f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fea1f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fea1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="fea1f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fea1f-117">Request headers</span></span>
| <span data-ttu-id="fea1f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fea1f-118">Name</span></span>       | <span data-ttu-id="fea1f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fea1f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fea1f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fea1f-120">Authorization</span></span>  | <span data-ttu-id="fea1f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fea1f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fea1f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fea1f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fea1f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fea1f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fea1f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fea1f-126">Request body</span></span>
<span data-ttu-id="fea1f-127">No corpo da solicitação, fornece uma representação JSON do objeto [WorkbookChart](../resources/chart.md) .</span><span class="sxs-lookup"><span data-stu-id="fea1f-127">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fea1f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea1f-128">Response</span></span>

<span data-ttu-id="fea1f-129">Se tiver êxito, este método retornará `201 Created` código de resposta e o objeto [WorkbookChart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fea1f-129">If successful, this method returns `201 Created` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fea1f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fea1f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fea1f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fea1f-131">Request</span></span>
<span data-ttu-id="fea1f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fea1f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="fea1f-133">No corpo da solicitação, fornece uma representação JSON do objeto [WorkbookChart](../resources/chart.md) .</span><span class="sxs-lookup"><span data-stu-id="fea1f-133">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fea1f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea1f-134">Response</span></span>
<span data-ttu-id="fea1f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fea1f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->