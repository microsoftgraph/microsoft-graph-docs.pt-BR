---
title: Atualizar chartaxistitle
description: Atualiza as propriedades do objeto chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2668e841c6628e779d296696be7b2fbe9344b4aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853981"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="94be3-103">Atualizar chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="94be3-103">Update chartaxistitle</span></span>

> <span data-ttu-id="94be3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="94be3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94be3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="94be3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94be3-106">Atualiza as propriedades do objeto chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="94be3-106">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94be3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="94be3-107">Permissions</span></span>
<span data-ttu-id="94be3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94be3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94be3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94be3-110">Permission type</span></span>      | <span data-ttu-id="94be3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94be3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94be3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94be3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94be3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94be3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94be3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94be3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94be3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94be3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94be3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94be3-116">Application</span></span> | <span data-ttu-id="94be3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94be3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94be3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94be3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="94be3-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="94be3-119">Optional request headers</span></span>
| <span data-ttu-id="94be3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="94be3-120">Name</span></span>       | <span data-ttu-id="94be3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="94be3-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="94be3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94be3-122">Authorization</span></span>  | <span data-ttu-id="94be3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94be3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94be3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="94be3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="94be3-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="94be3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94be3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94be3-128">Request body</span></span>
<span data-ttu-id="94be3-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="94be3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94be3-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94be3-132">Property</span></span>     | <span data-ttu-id="94be3-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="94be3-133">Type</span></span>   |<span data-ttu-id="94be3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="94be3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94be3-135">texto</span><span class="sxs-lookup"><span data-stu-id="94be3-135">text</span></span>|<span data-ttu-id="94be3-136">string</span><span class="sxs-lookup"><span data-stu-id="94be3-136">string</span></span>|<span data-ttu-id="94be3-137">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="94be3-137">Represents the axis title.</span></span>|
|<span data-ttu-id="94be3-138">visible</span><span class="sxs-lookup"><span data-stu-id="94be3-138">visible</span></span>|<span data-ttu-id="94be3-139">booliano</span><span class="sxs-lookup"><span data-stu-id="94be3-139">boolean</span></span>|<span data-ttu-id="94be3-140">Um booliano que especifica a visibilidade de um título do eixo.</span><span class="sxs-lookup"><span data-stu-id="94be3-140">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="94be3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="94be3-141">Response</span></span>

<span data-ttu-id="94be3-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartAxisTitle](../resources/chartaxistitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94be3-142">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94be3-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94be3-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94be3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94be3-144">Request</span></span>
<span data-ttu-id="94be3-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94be3-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="94be3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="94be3-146">Response</span></span>
<span data-ttu-id="94be3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94be3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
