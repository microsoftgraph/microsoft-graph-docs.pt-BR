---
title: Atualizar charttitle
description: Atualiza as propriedades do objeto charttitle.
ms.openlocfilehash: a20cafee793c5622fe29ad57aafb8e3d1e5cd2b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034009"
---
# <a name="update-charttitle"></a><span data-ttu-id="380b3-103">Atualizar charttitle</span><span class="sxs-lookup"><span data-stu-id="380b3-103">Update charttitle</span></span>

> <span data-ttu-id="380b3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="380b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="380b3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="380b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="380b3-106">Atualiza as propriedades do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="380b3-106">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="380b3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="380b3-107">Permissions</span></span>
<span data-ttu-id="380b3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="380b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="380b3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="380b3-110">Permission type</span></span>      | <span data-ttu-id="380b3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="380b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="380b3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="380b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="380b3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="380b3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="380b3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="380b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="380b3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="380b3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="380b3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="380b3-116">Application</span></span> | <span data-ttu-id="380b3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="380b3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="380b3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="380b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="380b3-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="380b3-119">Optional request headers</span></span>
| <span data-ttu-id="380b3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="380b3-120">Name</span></span>       | <span data-ttu-id="380b3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="380b3-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="380b3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="380b3-122">Authorization</span></span>  | <span data-ttu-id="380b3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="380b3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="380b3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="380b3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="380b3-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="380b3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="380b3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="380b3-128">Request body</span></span>
<span data-ttu-id="380b3-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="380b3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="380b3-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="380b3-132">Property</span></span>     | <span data-ttu-id="380b3-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="380b3-133">Type</span></span>   |<span data-ttu-id="380b3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="380b3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="380b3-135">overlay</span><span class="sxs-lookup"><span data-stu-id="380b3-135">overlay</span></span>|<span data-ttu-id="380b3-136">booliano</span><span class="sxs-lookup"><span data-stu-id="380b3-136">boolean</span></span>|<span data-ttu-id="380b3-137">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="380b3-137">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="380b3-138">texto</span><span class="sxs-lookup"><span data-stu-id="380b3-138">text</span></span>|<span data-ttu-id="380b3-139">string</span><span class="sxs-lookup"><span data-stu-id="380b3-139">string</span></span>|<span data-ttu-id="380b3-140">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="380b3-140">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="380b3-141">visible</span><span class="sxs-lookup"><span data-stu-id="380b3-141">visible</span></span>|<span data-ttu-id="380b3-142">booliano</span><span class="sxs-lookup"><span data-stu-id="380b3-142">boolean</span></span>|<span data-ttu-id="380b3-143">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="380b3-143">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="380b3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="380b3-144">Response</span></span>

<span data-ttu-id="380b3-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartTitle](../resources/charttitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="380b3-145">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="380b3-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="380b3-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="380b3-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="380b3-147">Request</span></span>
<span data-ttu-id="380b3-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="380b3-148">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="380b3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="380b3-149">Response</span></span>
<span data-ttu-id="380b3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="380b3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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