---
title: Lista de tendências
description: Percepção calculada que retorna a lista de itens de tendências em torno do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: bc0dcd70ef8fb527096e8142f188f9c2cbf02193
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926215"
---
# <a name="list-trending"></a><span data-ttu-id="5f52d-103">Lista de tendências</span><span class="sxs-lookup"><span data-stu-id="5f52d-103">List trending</span></span>

> <span data-ttu-id="5f52d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f52d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f52d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f52d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f52d-106">Percepção calculada que retorna a lista de itens de tendências em torno do usuário.</span><span class="sxs-lookup"><span data-stu-id="5f52d-106">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f52d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5f52d-107">Permissions</span></span>
<span data-ttu-id="5f52d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f52d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5f52d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f52d-110">Permission type</span></span>      | <span data-ttu-id="5f52d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f52d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f52d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f52d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5f52d-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f52d-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5f52d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f52d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f52d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f52d-115">Not supported.</span></span>    |
|<span data-ttu-id="5f52d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f52d-116">Application</span></span> | <span data-ttu-id="5f52d-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f52d-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f52d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f52d-118">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f52d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f52d-119">Optional query parameters</span></span>
<span data-ttu-id="5f52d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f52d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5f52d-121">Você pode usar o `$filter` parâmetro para filtrar itens de tendências de consulta.</span><span class="sxs-lookup"><span data-stu-id="5f52d-121">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="5f52d-122">Por exemplo, com base no tipo:</span><span class="sxs-lookup"><span data-stu-id="5f52d-122">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="5f52d-123">Ou com base no tipo de contêiner:</span><span class="sxs-lookup"><span data-stu-id="5f52d-123">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="5f52d-124">Consulte os tipos de contêiner e os tipos que você pode filtrar por em [resourceVisualization](../resources/insights-resourcevisualization.md)a disponíveis.</span><span class="sxs-lookup"><span data-stu-id="5f52d-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="5f52d-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f52d-125">Request headers</span></span>
| <span data-ttu-id="5f52d-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f52d-126">Header</span></span>       |  <span data-ttu-id="5f52d-127">Valor</span><span class="sxs-lookup"><span data-stu-id="5f52d-127">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="5f52d-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f52d-128">Authorization</span></span>  | <span data-ttu-id="5f52d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f52d-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5f52d-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f52d-131">Accept</span></span>  | <span data-ttu-id="5f52d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="5f52d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f52d-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f52d-133">Request body</span></span>
<span data-ttu-id="5f52d-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f52d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f52d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f52d-135">Response</span></span>

<span data-ttu-id="5f52d-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de itens [de tendências](../resources/insights-trending.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f52d-136">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="5f52d-137">Cada item contém propriedades de visualização para exibir o item em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="5f52d-137">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="5f52d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f52d-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5f52d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f52d-139">Request</span></span>
<span data-ttu-id="5f52d-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f52d-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="5f52d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f52d-141">Response</span></span>
<span data-ttu-id="5f52d-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f52d-142">Here is an example of the response.</span></span> <span data-ttu-id="5f52d-143">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="5f52d-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5f52d-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f52d-144">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="5f52d-145">Consulte uma resposta de exemplo não truncado na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="5f52d-145">See an example un-truncated response at the bottom of the page.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="5f52d-146">A expansão de recurso</span><span class="sxs-lookup"><span data-stu-id="5f52d-146">Expanding resource</span></span>
<span data-ttu-id="5f52d-147">O recurso referenciado por um insight tendência pode ser expandido.</span><span class="sxs-lookup"><span data-stu-id="5f52d-147">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
