---
title: Atualizar chartaxis
description: Atualiza as propriedades do objeto chartaxis.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 843aad2b3d6ea822078834439a085ba4bb10bf8b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813696"
---
# <a name="update-chartaxis"></a><span data-ttu-id="f5e21-103">Atualizar chartaxis</span><span class="sxs-lookup"><span data-stu-id="f5e21-103">Update chartaxis</span></span>

> <span data-ttu-id="f5e21-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5e21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5e21-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5e21-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5e21-106">Atualiza as propriedades do objeto chartaxis.</span><span class="sxs-lookup"><span data-stu-id="f5e21-106">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5e21-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5e21-107">Permissions</span></span>
<span data-ttu-id="f5e21-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5e21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5e21-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5e21-110">Permission type</span></span>      | <span data-ttu-id="f5e21-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5e21-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5e21-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5e21-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5e21-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5e21-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5e21-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5e21-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5e21-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5e21-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5e21-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5e21-116">Application</span></span> | <span data-ttu-id="f5e21-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5e21-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5e21-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5e21-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="f5e21-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f5e21-119">Optional request headers</span></span>
| <span data-ttu-id="f5e21-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f5e21-120">Name</span></span>       | <span data-ttu-id="f5e21-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5e21-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f5e21-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5e21-122">Authorization</span></span>  | <span data-ttu-id="f5e21-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5e21-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5e21-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f5e21-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f5e21-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f5e21-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5e21-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e21-128">Request body</span></span>
<span data-ttu-id="f5e21-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f5e21-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f5e21-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5e21-132">Property</span></span>     | <span data-ttu-id="f5e21-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5e21-133">Type</span></span>   |<span data-ttu-id="f5e21-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5e21-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5e21-135">majorUnit</span><span class="sxs-lookup"><span data-stu-id="f5e21-135">majorUnit</span></span>|<span data-ttu-id="f5e21-136">object</span><span class="sxs-lookup"><span data-stu-id="f5e21-136">object</span></span>|<span data-ttu-id="f5e21-p106">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="f5e21-p106">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="f5e21-140">maximum</span><span class="sxs-lookup"><span data-stu-id="f5e21-140">maximum</span></span>|<span data-ttu-id="f5e21-141">object</span><span class="sxs-lookup"><span data-stu-id="f5e21-141">object</span></span>|<span data-ttu-id="f5e21-p107">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="f5e21-p107">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f5e21-145">minimum</span><span class="sxs-lookup"><span data-stu-id="f5e21-145">minimum</span></span>|<span data-ttu-id="f5e21-146">object</span><span class="sxs-lookup"><span data-stu-id="f5e21-146">object</span></span>|<span data-ttu-id="f5e21-p108">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="f5e21-p108">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f5e21-150">minorUnit</span><span class="sxs-lookup"><span data-stu-id="f5e21-150">minorUnit</span></span>|<span data-ttu-id="f5e21-151">object</span><span class="sxs-lookup"><span data-stu-id="f5e21-151">object</span></span>|<span data-ttu-id="f5e21-p109">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="f5e21-p109">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="f5e21-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5e21-155">Response</span></span>

<span data-ttu-id="f5e21-156">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartAxis](../resources/chartaxis.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5e21-156">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5e21-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5e21-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5e21-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e21-158">Request</span></span>
<span data-ttu-id="f5e21-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5e21-159">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f5e21-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5e21-160">Response</span></span>
<span data-ttu-id="f5e21-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5e21-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
