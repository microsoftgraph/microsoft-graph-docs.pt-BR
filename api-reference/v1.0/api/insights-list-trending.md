---
title: Listar tendências
description: Insights calculados que retornam a lista de itens de tendências do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: f0853d4a215fcb554243a724b1d53d74f848a81d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516707"
---
# <a name="list-trending"></a><span data-ttu-id="ab129-103">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="ab129-103">List trending</span></span>

<span data-ttu-id="ab129-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab129-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab129-105">Informação calculada que inclui uma lista de documentos que envolvem a tendência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ab129-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab129-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab129-106">Permissions</span></span>
<span data-ttu-id="ab129-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab129-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ab129-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab129-109">Permission type</span></span>      | <span data-ttu-id="ab129-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab129-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab129-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab129-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ab129-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab129-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab129-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab129-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab129-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab129-114">Not supported.</span></span>    |
|<span data-ttu-id="ab129-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab129-115">Application</span></span> | <span data-ttu-id="ab129-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab129-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab129-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab129-117">HTTP request</span></span>
<span data-ttu-id="ab129-118">Obter uma lista de documentos de tendências em torno do usuário conectado ou do usuário especificado:</span><span class="sxs-lookup"><span data-stu-id="ab129-118">Get a list of documents trending around the signed-in user or specified user:</span></span>

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="ab129-119">Expanda o recurso mencionado por uma visão de **tendências** :</span><span class="sxs-lookup"><span data-stu-id="ab129-119">Expand the resource referenced by a **trending** insight:</span></span>

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab129-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab129-120">Optional query parameters</span></span>
<span data-ttu-id="ab129-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab129-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ab129-122">Você pode usar o `$filter` parâmetro de consulta para filtrar itens de tendência.</span><span class="sxs-lookup"><span data-stu-id="ab129-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="ab129-123">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="ab129-123">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="ab129-124">Ou com base no **ContainerType**:</span><span class="sxs-lookup"><span data-stu-id="ab129-124">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="ab129-125">Confira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="ab129-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="ab129-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab129-126">Request headers</span></span>
| <span data-ttu-id="ab129-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab129-127">Header</span></span>       |  <span data-ttu-id="ab129-128">Valor</span><span class="sxs-lookup"><span data-stu-id="ab129-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="ab129-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab129-129">Authorization</span></span>  | <span data-ttu-id="ab129-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab129-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ab129-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab129-132">Accept</span></span>  | <span data-ttu-id="ab129-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ab129-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab129-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab129-134">Request body</span></span>
<span data-ttu-id="ab129-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab129-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab129-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab129-136">Response</span></span>

<span data-ttu-id="ab129-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens de [tendência](../resources/insights-trending.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab129-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="ab129-138">Cada item contém propriedades de visualização para exibir o item em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="ab129-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="ab129-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab129-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ab129-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab129-140">Request</span></span>
<span data-ttu-id="ab129-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab129-141">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="ab129-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab129-142">Response</span></span>
<span data-ttu-id="ab129-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab129-143">Here is an example of the response.</span></span> <span data-ttu-id="ab129-144">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="ab129-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ab129-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab129-145">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="ab129-146">Veja um exemplo de resposta un truncada na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="ab129-146">See an example un-truncated response at the bottom of the page.</span></span>
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


