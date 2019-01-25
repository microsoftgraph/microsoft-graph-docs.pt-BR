---
title: Atualizar chartaxis
description: Atualiza as propriedades do objeto chartaxis.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9eb7f4cd2ddf1408f818eff78b7dc4d86a62376c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519455"
---
# <a name="update-chartaxis"></a><span data-ttu-id="02629-103">Atualizar chartaxis</span><span class="sxs-lookup"><span data-stu-id="02629-103">Update chartaxis</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02629-104">Atualiza as propriedades do objeto chartaxis.</span><span class="sxs-lookup"><span data-stu-id="02629-104">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="02629-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="02629-105">Permissions</span></span>
<span data-ttu-id="02629-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02629-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02629-108">Permission type</span></span>      | <span data-ttu-id="02629-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02629-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02629-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02629-110">Delegated (work or school account)</span></span> | <span data-ttu-id="02629-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02629-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="02629-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02629-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02629-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02629-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="02629-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02629-114">Application</span></span> | <span data-ttu-id="02629-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02629-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02629-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02629-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="02629-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="02629-117">Optional request headers</span></span>
| <span data-ttu-id="02629-118">Nome</span><span class="sxs-lookup"><span data-stu-id="02629-118">Name</span></span>       | <span data-ttu-id="02629-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="02629-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="02629-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="02629-120">Authorization</span></span>  | <span data-ttu-id="02629-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02629-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02629-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="02629-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="02629-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="02629-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02629-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02629-126">Request body</span></span>
<span data-ttu-id="02629-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="02629-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="02629-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02629-130">Property</span></span>     | <span data-ttu-id="02629-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02629-131">Type</span></span>   |<span data-ttu-id="02629-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02629-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02629-133">majorUnit</span><span class="sxs-lookup"><span data-stu-id="02629-133">majorUnit</span></span>|<span data-ttu-id="02629-134">objeto</span><span class="sxs-lookup"><span data-stu-id="02629-134">object</span></span>|<span data-ttu-id="02629-p105">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="02629-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="02629-138">maximum</span><span class="sxs-lookup"><span data-stu-id="02629-138">maximum</span></span>|<span data-ttu-id="02629-139">objeto</span><span class="sxs-lookup"><span data-stu-id="02629-139">object</span></span>|<span data-ttu-id="02629-p106">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="02629-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="02629-143">minimum</span><span class="sxs-lookup"><span data-stu-id="02629-143">minimum</span></span>|<span data-ttu-id="02629-144">objeto</span><span class="sxs-lookup"><span data-stu-id="02629-144">object</span></span>|<span data-ttu-id="02629-p107">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="02629-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="02629-148">minorUnit</span><span class="sxs-lookup"><span data-stu-id="02629-148">minorUnit</span></span>|<span data-ttu-id="02629-149">object</span><span class="sxs-lookup"><span data-stu-id="02629-149">object</span></span>|<span data-ttu-id="02629-p108">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="02629-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="02629-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="02629-153">Response</span></span>

<span data-ttu-id="02629-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartAxis](../resources/chartaxis.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02629-154">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02629-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02629-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02629-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02629-156">Request</span></span>
<span data-ttu-id="02629-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02629-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="02629-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="02629-158">Response</span></span>
<span data-ttu-id="02629-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02629-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartaxis-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
