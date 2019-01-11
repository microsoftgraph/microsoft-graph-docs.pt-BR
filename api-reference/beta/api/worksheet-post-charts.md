---
title: Criar gráfico
description: Use esta API para criar um novo gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 96d5d53254ae9874a96dc6bfc5440991619ac6a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894450"
---
# <a name="create-chart"></a><span data-ttu-id="89848-103">Criar gráfico</span><span class="sxs-lookup"><span data-stu-id="89848-103">Create Chart</span></span>

> <span data-ttu-id="89848-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="89848-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89848-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="89848-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89848-106">Use esta API para criar um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="89848-106">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="89848-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="89848-107">Permissions</span></span>
<span data-ttu-id="89848-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89848-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89848-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89848-110">Permission type</span></span>      | <span data-ttu-id="89848-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89848-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89848-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89848-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89848-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89848-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89848-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89848-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89848-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89848-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89848-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89848-116">Application</span></span> | <span data-ttu-id="89848-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89848-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89848-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89848-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="89848-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89848-119">Request headers</span></span>
| <span data-ttu-id="89848-120">Nome</span><span class="sxs-lookup"><span data-stu-id="89848-120">Name</span></span>       | <span data-ttu-id="89848-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="89848-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89848-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="89848-122">Authorization</span></span>  | <span data-ttu-id="89848-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89848-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="89848-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="89848-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="89848-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="89848-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89848-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89848-128">Request body</span></span>
<span data-ttu-id="89848-129">No corpo da solicitação, forneça uma representação JSON do objeto [Chart](../resources/chart.md).</span><span class="sxs-lookup"><span data-stu-id="89848-129">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="89848-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="89848-130">Response</span></span>

<span data-ttu-id="89848-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89848-131">If successful, this method returns `201 Created` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89848-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89848-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89848-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89848-133">Request</span></span>
<span data-ttu-id="89848-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89848-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="89848-135">No corpo da solicitação, forneça uma representação JSON do objeto [Chart](../resources/chart.md).</span><span class="sxs-lookup"><span data-stu-id="89848-135">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="89848-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="89848-136">Response</span></span>
<span data-ttu-id="89848-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89848-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
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
