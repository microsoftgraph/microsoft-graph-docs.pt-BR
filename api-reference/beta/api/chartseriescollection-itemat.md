---
title: 'ChartSeriesCollection: ItemAt'
description: Recupera uma série com base na respectiva posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a564a23161cac3a8c750223a75c6fee4ad429b1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936428"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="16a80-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="16a80-103">ChartSeriesCollection: ItemAt</span></span>

> <span data-ttu-id="16a80-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16a80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16a80-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16a80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16a80-106">Recupera uma série com base na respectiva posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="16a80-106">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="16a80-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16a80-107">Permissions</span></span>
<span data-ttu-id="16a80-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16a80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16a80-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16a80-110">Permission type</span></span>      | <span data-ttu-id="16a80-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16a80-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16a80-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16a80-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16a80-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16a80-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16a80-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16a80-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16a80-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16a80-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16a80-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16a80-116">Application</span></span> | <span data-ttu-id="16a80-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16a80-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16a80-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16a80-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="16a80-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16a80-119">Request headers</span></span>
| <span data-ttu-id="16a80-120">Nome</span><span class="sxs-lookup"><span data-stu-id="16a80-120">Name</span></span>       | <span data-ttu-id="16a80-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="16a80-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="16a80-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16a80-122">Authorization</span></span>  | <span data-ttu-id="16a80-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16a80-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16a80-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="16a80-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="16a80-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="16a80-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16a80-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16a80-128">Request body</span></span>
<span data-ttu-id="16a80-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16a80-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="16a80-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="16a80-130">Parameter</span></span>    | <span data-ttu-id="16a80-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="16a80-131">Type</span></span>   |<span data-ttu-id="16a80-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="16a80-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16a80-133">índice</span><span class="sxs-lookup"><span data-stu-id="16a80-133">index</span></span>|<span data-ttu-id="16a80-134">number</span><span class="sxs-lookup"><span data-stu-id="16a80-134">number</span></span>|<span data-ttu-id="16a80-p105">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="16a80-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="16a80-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="16a80-137">Response</span></span>

<span data-ttu-id="16a80-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16a80-138">If successful, this method returns `200 OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16a80-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16a80-139">Example</span></span>
<span data-ttu-id="16a80-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="16a80-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="16a80-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16a80-141">Request</span></span>
<span data-ttu-id="16a80-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16a80-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="16a80-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="16a80-143">Response</span></span>
<span data-ttu-id="16a80-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16a80-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
