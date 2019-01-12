---
title: Atualizar charttitle
description: Atualiza as propriedades do objeto charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4d0beb65acb208d6f04d495a98b3c48a046b29ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980801"
---
# <a name="update-charttitle"></a><span data-ttu-id="c0585-103">Atualizar charttitle</span><span class="sxs-lookup"><span data-stu-id="c0585-103">Update charttitle</span></span>

> <span data-ttu-id="c0585-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0585-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0585-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0585-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0585-106">Atualiza as propriedades do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="c0585-106">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0585-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0585-107">Permissions</span></span>
<span data-ttu-id="c0585-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0585-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0585-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0585-110">Permission type</span></span>      | <span data-ttu-id="c0585-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0585-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0585-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0585-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0585-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0585-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0585-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0585-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0585-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0585-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0585-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0585-116">Application</span></span> | <span data-ttu-id="c0585-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0585-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0585-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0585-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="c0585-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c0585-119">Optional request headers</span></span>
| <span data-ttu-id="c0585-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c0585-120">Name</span></span>       | <span data-ttu-id="c0585-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0585-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c0585-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0585-122">Authorization</span></span>  | <span data-ttu-id="c0585-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0585-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0585-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c0585-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c0585-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c0585-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0585-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0585-128">Request body</span></span>
<span data-ttu-id="c0585-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c0585-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0585-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0585-132">Property</span></span>     | <span data-ttu-id="c0585-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0585-133">Type</span></span>   |<span data-ttu-id="c0585-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0585-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0585-135">overlay</span><span class="sxs-lookup"><span data-stu-id="c0585-135">overlay</span></span>|<span data-ttu-id="c0585-136">booliano</span><span class="sxs-lookup"><span data-stu-id="c0585-136">boolean</span></span>|<span data-ttu-id="c0585-137">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="c0585-137">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="c0585-138">texto</span><span class="sxs-lookup"><span data-stu-id="c0585-138">text</span></span>|<span data-ttu-id="c0585-139">string</span><span class="sxs-lookup"><span data-stu-id="c0585-139">string</span></span>|<span data-ttu-id="c0585-140">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="c0585-140">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="c0585-141">visible</span><span class="sxs-lookup"><span data-stu-id="c0585-141">visible</span></span>|<span data-ttu-id="c0585-142">booliano</span><span class="sxs-lookup"><span data-stu-id="c0585-142">boolean</span></span>|<span data-ttu-id="c0585-143">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="c0585-143">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="c0585-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0585-144">Response</span></span>

<span data-ttu-id="c0585-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartTitle](../resources/charttitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0585-145">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0585-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0585-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0585-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0585-147">Request</span></span>
<span data-ttu-id="c0585-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0585-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="c0585-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0585-149">Response</span></span>
<span data-ttu-id="c0585-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0585-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
