---
title: Atualizar chartlegend
description: Atualiza as propriedades do objeto chartlegend.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a5dae3bfc8244a0f622665d831c3081e1f0f432d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854632"
---
# <a name="update-chartlegend"></a><span data-ttu-id="f7198-103">Atualizar chartlegend</span><span class="sxs-lookup"><span data-stu-id="f7198-103">Update chartlegend</span></span>

> <span data-ttu-id="f7198-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f7198-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7198-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f7198-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7198-106">Atualiza as propriedades do objeto chartlegend.</span><span class="sxs-lookup"><span data-stu-id="f7198-106">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7198-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7198-107">Permissions</span></span>
<span data-ttu-id="f7198-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7198-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7198-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7198-110">Permission type</span></span>      | <span data-ttu-id="f7198-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7198-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7198-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7198-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7198-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7198-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7198-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7198-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7198-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7198-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7198-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7198-116">Application</span></span> | <span data-ttu-id="f7198-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7198-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7198-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7198-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="f7198-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f7198-119">Optional request headers</span></span>
| <span data-ttu-id="f7198-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f7198-120">Name</span></span>       | <span data-ttu-id="f7198-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7198-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f7198-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7198-122">Authorization</span></span>  | <span data-ttu-id="f7198-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7198-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7198-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f7198-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f7198-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f7198-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7198-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7198-128">Request body</span></span>
<span data-ttu-id="f7198-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f7198-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f7198-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7198-132">Property</span></span>     | <span data-ttu-id="f7198-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7198-133">Type</span></span>   |<span data-ttu-id="f7198-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7198-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7198-135">overlay</span><span class="sxs-lookup"><span data-stu-id="f7198-135">overlay</span></span>|<span data-ttu-id="f7198-136">booliano</span><span class="sxs-lookup"><span data-stu-id="f7198-136">boolean</span></span>|<span data-ttu-id="f7198-137">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="f7198-137">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="f7198-138">position</span><span class="sxs-lookup"><span data-stu-id="f7198-138">position</span></span>|<span data-ttu-id="f7198-139">string</span><span class="sxs-lookup"><span data-stu-id="f7198-139">string</span></span>|<span data-ttu-id="f7198-p106">Representa a posição da legenda no gráfico. Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner` e `Custom`.</span><span class="sxs-lookup"><span data-stu-id="f7198-p106">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="f7198-142">visible</span><span class="sxs-lookup"><span data-stu-id="f7198-142">visible</span></span>|<span data-ttu-id="f7198-143">booliano</span><span class="sxs-lookup"><span data-stu-id="f7198-143">boolean</span></span>|<span data-ttu-id="f7198-144">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="f7198-144">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="f7198-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7198-145">Response</span></span>

<span data-ttu-id="f7198-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartLegend](../resources/chartlegend.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7198-146">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7198-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7198-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7198-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7198-148">Request</span></span>
<span data-ttu-id="f7198-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7198-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="f7198-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7198-150">Response</span></span>
<span data-ttu-id="f7198-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7198-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
