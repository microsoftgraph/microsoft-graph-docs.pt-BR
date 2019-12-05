---
title: Listar tendências
description: Insights calculados que retornam a lista de itens de tendências do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: e97e5f9a72084b7748551d60e795e43e80f353ed
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844330"
---
# <a name="list-trending"></a><span data-ttu-id="f8095-103">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="f8095-103">List trending</span></span>

<span data-ttu-id="f8095-104">Informação calculada que inclui uma lista de documentos que envolvem a tendência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f8095-104">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8095-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8095-105">Permissions</span></span>
<span data-ttu-id="f8095-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f8095-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8095-108">Permission type</span></span>      | <span data-ttu-id="f8095-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8095-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8095-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8095-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f8095-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8095-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f8095-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8095-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8095-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8095-113">Not supported.</span></span>    |
|<span data-ttu-id="f8095-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8095-114">Application</span></span> | <span data-ttu-id="f8095-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8095-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8095-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8095-116">HTTP request</span></span>
<span data-ttu-id="f8095-117">Obter uma lista de documentos de tendências em torno do usuário conectado ou do usuário especificado:</span><span class="sxs-lookup"><span data-stu-id="f8095-117">Get a list of documents trending around the signed-in user or specified user:</span></span>

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="f8095-118">Expanda o recurso mencionado por uma visão de **tendências** :</span><span class="sxs-lookup"><span data-stu-id="f8095-118">Expand the resource referenced by a **trending** insight:</span></span>

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8095-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f8095-119">Optional query parameters</span></span>
<span data-ttu-id="f8095-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f8095-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f8095-121">Você pode usar o `$filter` parâmetro de consulta para filtrar itens de tendência.</span><span class="sxs-lookup"><span data-stu-id="f8095-121">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="f8095-122">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="f8095-122">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="f8095-123">Ou com base no **ContainerType**:</span><span class="sxs-lookup"><span data-stu-id="f8095-123">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="f8095-124">Confira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="f8095-124">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="f8095-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8095-125">Request headers</span></span>
| <span data-ttu-id="f8095-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8095-126">Header</span></span>       |  <span data-ttu-id="f8095-127">Valor</span><span class="sxs-lookup"><span data-stu-id="f8095-127">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="f8095-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8095-128">Authorization</span></span>  | <span data-ttu-id="f8095-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8095-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f8095-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8095-131">Accept</span></span>  | <span data-ttu-id="f8095-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f8095-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8095-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8095-133">Request body</span></span>
<span data-ttu-id="f8095-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8095-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8095-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8095-135">Response</span></span>

<span data-ttu-id="f8095-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens de [tendência](../resources/insights-trending.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8095-136">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="f8095-137">Cada item contém propriedades de visualização para exibir o item em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="f8095-137">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="f8095-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8095-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f8095-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8095-139">Request</span></span>
<span data-ttu-id="f8095-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8095-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="f8095-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8095-141">Response</span></span>
<span data-ttu-id="f8095-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8095-142">Here is an example of the response.</span></span> <span data-ttu-id="f8095-143">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f8095-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f8095-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8095-144">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="f8095-145">Veja um exemplo de resposta un truncada na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="f8095-145">See an example un-truncated response at the bottom of the page.</span></span>
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


