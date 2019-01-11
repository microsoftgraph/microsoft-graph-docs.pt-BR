---
title: 'ChartPointsCollection: ItemAt'
description: Recupera um ponto com base na respectiva posição dentro da série.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c497f0f15b3d1ddcdb3e5adb05d9e9d0b1ade57e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829012"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="cef00-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="cef00-103">ChartPointsCollection: ItemAt</span></span>

> <span data-ttu-id="cef00-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cef00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cef00-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cef00-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cef00-106">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="cef00-106">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="cef00-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cef00-107">Permissions</span></span>
<span data-ttu-id="cef00-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cef00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cef00-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cef00-110">Permission type</span></span>      | <span data-ttu-id="cef00-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cef00-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cef00-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cef00-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cef00-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cef00-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cef00-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cef00-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cef00-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cef00-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cef00-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cef00-116">Application</span></span> | <span data-ttu-id="cef00-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cef00-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cef00-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cef00-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="cef00-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cef00-119">Request headers</span></span>
| <span data-ttu-id="cef00-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cef00-120">Name</span></span>       | <span data-ttu-id="cef00-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cef00-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cef00-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cef00-122">Authorization</span></span>  | <span data-ttu-id="cef00-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cef00-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cef00-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cef00-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cef00-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="cef00-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cef00-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cef00-128">Request body</span></span>
<span data-ttu-id="cef00-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cef00-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cef00-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cef00-130">Parameter</span></span>    | <span data-ttu-id="cef00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cef00-131">Type</span></span>   |<span data-ttu-id="cef00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cef00-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cef00-133">índice</span><span class="sxs-lookup"><span data-stu-id="cef00-133">index</span></span>|<span data-ttu-id="cef00-134">number</span><span class="sxs-lookup"><span data-stu-id="cef00-134">number</span></span>|<span data-ttu-id="cef00-p105">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="cef00-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="cef00-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cef00-137">Response</span></span>

<span data-ttu-id="cef00-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartPoint](../resources/chartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cef00-138">If successful, this method returns `200 OK` response code and [ChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cef00-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cef00-139">Example</span></span>
<span data-ttu-id="cef00-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="cef00-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cef00-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cef00-141">Request</span></span>
<span data-ttu-id="cef00-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cef00-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="cef00-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cef00-143">Response</span></span>
<span data-ttu-id="cef00-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cef00-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
