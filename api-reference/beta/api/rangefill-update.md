---
title: Atualizar rangefill
description: Atualize as propriedades do objeto rangefill.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 166550959cd6ce4b481b85d4dbff344f1a070ae5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836709"
---
# <a name="update-rangefill"></a><span data-ttu-id="c3266-103">Atualizar rangefill</span><span class="sxs-lookup"><span data-stu-id="c3266-103">Update rangefill</span></span>

> <span data-ttu-id="c3266-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c3266-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3266-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c3266-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3266-106">Atualize as propriedades do objeto rangefill.</span><span class="sxs-lookup"><span data-stu-id="c3266-106">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3266-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3266-107">Permissions</span></span>
<span data-ttu-id="c3266-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3266-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3266-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3266-110">Permission type</span></span>      | <span data-ttu-id="c3266-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3266-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3266-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3266-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c3266-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3266-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c3266-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3266-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3266-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3266-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c3266-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3266-116">Application</span></span> | <span data-ttu-id="c3266-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3266-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3266-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3266-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="c3266-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c3266-119">Optional request headers</span></span>
| <span data-ttu-id="c3266-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c3266-120">Name</span></span>       | <span data-ttu-id="c3266-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3266-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c3266-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3266-122">Authorization</span></span>  | <span data-ttu-id="c3266-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3266-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3266-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c3266-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c3266-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3266-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3266-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3266-128">Request body</span></span>
<span data-ttu-id="c3266-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c3266-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c3266-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3266-132">Property</span></span>     | <span data-ttu-id="c3266-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3266-133">Type</span></span>   |<span data-ttu-id="c3266-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3266-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3266-135">color</span><span class="sxs-lookup"><span data-stu-id="c3266-135">color</span></span>|<span data-ttu-id="c3266-136">string</span><span class="sxs-lookup"><span data-stu-id="c3266-136">string</span></span>|<span data-ttu-id="c3266-137">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="c3266-137">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="c3266-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3266-138">Response</span></span>

<span data-ttu-id="c3266-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFill](../resources/rangefill.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3266-139">If successful, this method returns a `200 OK` response code and updated [RangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3266-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3266-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3266-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3266-141">Request</span></span>
<span data-ttu-id="c3266-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3266-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="c3266-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3266-143">Response</span></span>
<span data-ttu-id="c3266-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3266-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
