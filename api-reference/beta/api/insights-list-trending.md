---
title: Listar tendências
description: Informações calculadas que retornam a lista de itens que se referem ao usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 49f777e77663a4c055e186860f791459db57ca9c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323664"
---
# <a name="list-trending"></a><span data-ttu-id="645b3-103">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="645b3-103">List trending</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="645b3-104">Informações calculadas que retornam a lista de itens que se referem ao usuário.</span><span class="sxs-lookup"><span data-stu-id="645b3-104">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="645b3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="645b3-105">Permissions</span></span>
<span data-ttu-id="645b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="645b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="645b3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="645b3-108">Permission type</span></span>      | <span data-ttu-id="645b3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="645b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="645b3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="645b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="645b3-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="645b3-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="645b3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="645b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="645b3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="645b3-113">Not supported.</span></span>    |
|<span data-ttu-id="645b3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="645b3-114">Application</span></span> | <span data-ttu-id="645b3-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="645b3-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="645b3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="645b3-116">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="645b3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="645b3-117">Optional query parameters</span></span>
<span data-ttu-id="645b3-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="645b3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="645b3-119">Você pode usar o `$filter` parâmetro de consulta para filtrar itens de tendência.</span><span class="sxs-lookup"><span data-stu-id="645b3-119">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="645b3-120">Por exemplo, com base no tipo:</span><span class="sxs-lookup"><span data-stu-id="645b3-120">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="645b3-121">Ou com base no tipo de contêiner:</span><span class="sxs-lookup"><span data-stu-id="645b3-121">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="645b3-122">ConFira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="645b3-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="645b3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="645b3-123">Request headers</span></span>
| <span data-ttu-id="645b3-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="645b3-124">Header</span></span>       |  <span data-ttu-id="645b3-125">Valor</span><span class="sxs-lookup"><span data-stu-id="645b3-125">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="645b3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="645b3-126">Authorization</span></span>  | <span data-ttu-id="645b3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="645b3-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="645b3-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="645b3-129">Accept</span></span>  | <span data-ttu-id="645b3-130">application/json</span><span class="sxs-lookup"><span data-stu-id="645b3-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="645b3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="645b3-131">Request body</span></span>
<span data-ttu-id="645b3-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="645b3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="645b3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="645b3-133">Response</span></span>

<span data-ttu-id="645b3-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens de [tendência](../resources/insights-trending.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="645b3-134">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="645b3-135">Cada item contém propriedades de visualização para exibir o item em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="645b3-135">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="645b3-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="645b3-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="645b3-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="645b3-137">Request</span></span>
<span data-ttu-id="645b3-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="645b3-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="645b3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="645b3-139">Response</span></span>
<span data-ttu-id="645b3-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="645b3-140">Here is an example of the response.</span></span> <span data-ttu-id="645b3-141">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="645b3-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="645b3-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="645b3-142">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="645b3-143">Veja um exemplo de resposta un truncada na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="645b3-143">See an example un-truncated response at the bottom of the page.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```

### <a name="expanding-resource"></a><span data-ttu-id="645b3-144">Expandindo recurso</span><span class="sxs-lookup"><span data-stu-id="645b3-144">Expanding resource</span></span>
<span data-ttu-id="645b3-145">O recurso mencionado por uma visão de tendências pode ser expandido.</span><span class="sxs-lookup"><span data-stu-id="645b3-145">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
