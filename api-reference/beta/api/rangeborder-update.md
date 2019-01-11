---
title: Atualizar rangeborder
description: Atualize as propriedades do objeto rangeborder.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 99db19208242ae25c94c081b4e43f9f8caa47e67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877053"
---
# <a name="update-rangeborder"></a><span data-ttu-id="23932-103">Atualizar rangeborder</span><span class="sxs-lookup"><span data-stu-id="23932-103">Update rangeborder</span></span>

> <span data-ttu-id="23932-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="23932-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23932-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="23932-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23932-106">Atualize as propriedades do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="23932-106">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="23932-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="23932-107">Permissions</span></span>
<span data-ttu-id="23932-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23932-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23932-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23932-110">Permission type</span></span>      | <span data-ttu-id="23932-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23932-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23932-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23932-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23932-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23932-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23932-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23932-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23932-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23932-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23932-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23932-116">Application</span></span> | <span data-ttu-id="23932-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23932-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23932-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23932-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="23932-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="23932-119">Optional request headers</span></span>
| <span data-ttu-id="23932-120">Nome</span><span class="sxs-lookup"><span data-stu-id="23932-120">Name</span></span>       | <span data-ttu-id="23932-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="23932-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="23932-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="23932-122">Authorization</span></span>  | <span data-ttu-id="23932-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23932-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23932-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="23932-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="23932-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="23932-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23932-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23932-128">Request body</span></span>
<span data-ttu-id="23932-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="23932-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="23932-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23932-132">Property</span></span>     | <span data-ttu-id="23932-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="23932-133">Type</span></span>   |<span data-ttu-id="23932-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="23932-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23932-135">color</span><span class="sxs-lookup"><span data-stu-id="23932-135">color</span></span>|<span data-ttu-id="23932-136">string</span><span class="sxs-lookup"><span data-stu-id="23932-136">string</span></span>|<span data-ttu-id="23932-137">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="23932-137">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="23932-138">style</span><span class="sxs-lookup"><span data-stu-id="23932-138">style</span></span>|<span data-ttu-id="23932-139">string</span><span class="sxs-lookup"><span data-stu-id="23932-139">string</span></span>|<span data-ttu-id="23932-p106">Uma das constantes de estilo de linha especificando o estilo de linha da borda. Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double` e `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="23932-p106">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="23932-142">weight</span><span class="sxs-lookup"><span data-stu-id="23932-142">weight</span></span>|<span data-ttu-id="23932-143">string</span><span class="sxs-lookup"><span data-stu-id="23932-143">string</span></span>|<span data-ttu-id="23932-p107">Especifica a espessura da borda em torno de um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium` e `Thick`.</span><span class="sxs-lookup"><span data-stu-id="23932-p107">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="23932-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="23932-146">Response</span></span>

<span data-ttu-id="23932-147">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeBorder](../resources/rangeborder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23932-147">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23932-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23932-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23932-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23932-149">Request</span></span>
<span data-ttu-id="23932-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23932-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="23932-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="23932-151">Response</span></span>
<span data-ttu-id="23932-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23932-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
