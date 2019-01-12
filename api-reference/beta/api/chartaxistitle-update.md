---
title: Atualizar chartaxistitle
description: Atualiza as propriedades do objeto chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fd6b38b2ff7b0c65ed58b97326c9bb1e63d34079
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966367"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="2fd0a-103">Atualizar chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="2fd0a-103">Update chartaxistitle</span></span>

> <span data-ttu-id="2fd0a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fd0a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2fd0a-106">Atualiza as propriedades do objeto chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-106">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2fd0a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fd0a-107">Permissions</span></span>
<span data-ttu-id="2fd0a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fd0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fd0a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fd0a-110">Permission type</span></span>      | <span data-ttu-id="2fd0a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fd0a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fd0a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fd0a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2fd0a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fd0a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2fd0a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fd0a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fd0a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fd0a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2fd0a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fd0a-116">Application</span></span> | <span data-ttu-id="2fd0a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fd0a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fd0a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="2fd0a-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2fd0a-119">Optional request headers</span></span>
| <span data-ttu-id="2fd0a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2fd0a-120">Name</span></span>       | <span data-ttu-id="2fd0a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd0a-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2fd0a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fd0a-122">Authorization</span></span>  | <span data-ttu-id="2fd0a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fd0a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2fd0a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2fd0a-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fd0a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fd0a-128">Request body</span></span>
<span data-ttu-id="2fd0a-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2fd0a-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fd0a-132">Property</span></span>     | <span data-ttu-id="2fd0a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fd0a-133">Type</span></span>   |<span data-ttu-id="2fd0a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd0a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fd0a-135">texto</span><span class="sxs-lookup"><span data-stu-id="2fd0a-135">text</span></span>|<span data-ttu-id="2fd0a-136">string</span><span class="sxs-lookup"><span data-stu-id="2fd0a-136">string</span></span>|<span data-ttu-id="2fd0a-137">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-137">Represents the axis title.</span></span>|
|<span data-ttu-id="2fd0a-138">visible</span><span class="sxs-lookup"><span data-stu-id="2fd0a-138">visible</span></span>|<span data-ttu-id="2fd0a-139">booliano</span><span class="sxs-lookup"><span data-stu-id="2fd0a-139">boolean</span></span>|<span data-ttu-id="2fd0a-140">Um booliano que especifica a visibilidade de um título do eixo.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-140">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="2fd0a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fd0a-141">Response</span></span>

<span data-ttu-id="2fd0a-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartAxisTitle](../resources/chartaxistitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-142">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fd0a-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fd0a-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fd0a-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fd0a-144">Request</span></span>
<span data-ttu-id="2fd0a-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-145">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2fd0a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fd0a-146">Response</span></span>
<span data-ttu-id="2fd0a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fd0a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
