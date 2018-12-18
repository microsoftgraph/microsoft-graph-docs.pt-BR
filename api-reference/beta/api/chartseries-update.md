---
title: Atualizar chartseries
description: Atualiza as propriedades do objeto chartseries.
author: lumine2008
ms.openlocfilehash: 69e6de2e6d332a63f4ea7b1cc23ca48032cbbaba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358951"
---
# <a name="update-chartseries"></a><span data-ttu-id="53b32-103">Atualizar chartseries</span><span class="sxs-lookup"><span data-stu-id="53b32-103">Update chartseries</span></span>

> <span data-ttu-id="53b32-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="53b32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53b32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="53b32-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53b32-106">Atualiza as propriedades do objeto chartseries.</span><span class="sxs-lookup"><span data-stu-id="53b32-106">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="53b32-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="53b32-107">Permissions</span></span>
<span data-ttu-id="53b32-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b32-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53b32-110">Permission type</span></span>      | <span data-ttu-id="53b32-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53b32-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53b32-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53b32-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53b32-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53b32-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53b32-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53b32-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53b32-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53b32-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53b32-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53b32-116">Application</span></span> | <span data-ttu-id="53b32-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53b32-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53b32-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53b32-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="53b32-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="53b32-119">Optional request headers</span></span>
| <span data-ttu-id="53b32-120">Nome</span><span class="sxs-lookup"><span data-stu-id="53b32-120">Name</span></span>       | <span data-ttu-id="53b32-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="53b32-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="53b32-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="53b32-122">Authorization</span></span>  | <span data-ttu-id="53b32-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53b32-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53b32-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="53b32-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="53b32-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="53b32-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b32-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53b32-128">Request body</span></span>
<span data-ttu-id="53b32-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="53b32-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="53b32-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53b32-132">Property</span></span>     | <span data-ttu-id="53b32-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="53b32-133">Type</span></span>   |<span data-ttu-id="53b32-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="53b32-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53b32-135">name</span><span class="sxs-lookup"><span data-stu-id="53b32-135">name</span></span>|<span data-ttu-id="53b32-136">string</span><span class="sxs-lookup"><span data-stu-id="53b32-136">string</span></span>|<span data-ttu-id="53b32-137">Representa o nome de uma série em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="53b32-137">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="53b32-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="53b32-138">Response</span></span>

<span data-ttu-id="53b32-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartSeries](../resources/chartseries.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53b32-139">If successful, this method returns a `200 OK` response code and updated [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53b32-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53b32-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53b32-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53b32-141">Request</span></span>
<span data-ttu-id="53b32-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53b32-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="53b32-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="53b32-143">Response</span></span>
<span data-ttu-id="53b32-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53b32-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->