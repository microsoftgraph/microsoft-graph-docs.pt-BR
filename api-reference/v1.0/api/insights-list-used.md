---
title: Listar usados
description: Visão calculada que retorna a lista de arquivos usados com um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: cf884aeefd17400a1c1b8601a6d0d38b81b4a2da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516700"
---
# <a name="list-used"></a><span data-ttu-id="d857a-103">Listar usados</span><span class="sxs-lookup"><span data-stu-id="d857a-103">List used</span></span>

<span data-ttu-id="d857a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d857a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d857a-105">Informações calculadas que incluem uma lista de documentos modificados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="d857a-105">Calculated insight that includes a list of documents the user has modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="d857a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d857a-106">Permissions</span></span>
<span data-ttu-id="d857a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d857a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d857a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d857a-109">Permission type</span></span>      | <span data-ttu-id="d857a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d857a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d857a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d857a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d857a-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d857a-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d857a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d857a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d857a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d857a-114">Not supported.</span></span>    |
|<span data-ttu-id="d857a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d857a-115">Application</span></span> | <span data-ttu-id="d857a-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d857a-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d857a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d857a-117">HTTP request</span></span>
<span data-ttu-id="d857a-118">Obter uma lista de documentos que o usuário conectado modificou:</span><span class="sxs-lookup"><span data-stu-id="d857a-118">Get a list of documents that the signed-in user has modified:</span></span>

```http
GET /me/insights/used
```

<span data-ttu-id="d857a-119">Obtém uma lista de documentos que o usuário especificado modificou.</span><span class="sxs-lookup"><span data-stu-id="d857a-119">Get a list of documents that the specified user has modified.</span></span>

><span data-ttu-id="d857a-120">**Observação**: a solicitação de documentos **usados** por outro usuário retorna resultados classificados por **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="d857a-120">**Note**: Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="d857a-121">**lastAccessedDateTime** é então definido como **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="d857a-121">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>
```http
GET /users/{id | userPrincipalName}/insights/used
```

<span data-ttu-id="d857a-122">Expanda o recurso mencionado por uma percepção **usada** :</span><span class="sxs-lookup"><span data-stu-id="d857a-122">Expand the resource referenced by a **used** insight:</span></span>

```http
GET /me/insights/used/{id}/resource
GET /users/{id | userPrincipalName}/insights/used/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d857a-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d857a-123">Optional query parameters</span></span>
<span data-ttu-id="d857a-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d857a-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d857a-125">Você pode usar o `$filter` parâmetro de consulta para filtrar itens usados.</span><span class="sxs-lookup"><span data-stu-id="d857a-125">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="d857a-126">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="d857a-126">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="d857a-127">Ou com base no **ContainerType**:</span><span class="sxs-lookup"><span data-stu-id="d857a-127">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="d857a-128">Confira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="d857a-128">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="d857a-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d857a-129">Request headers</span></span>
| <span data-ttu-id="d857a-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d857a-130">Header</span></span>       |  <span data-ttu-id="d857a-131">Valor</span><span class="sxs-lookup"><span data-stu-id="d857a-131">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="d857a-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d857a-132">Authorization</span></span>  | <span data-ttu-id="d857a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d857a-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d857a-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d857a-135">Accept</span></span>  | <span data-ttu-id="d857a-136">application/json</span><span class="sxs-lookup"><span data-stu-id="d857a-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d857a-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d857a-137">Request body</span></span>
<span data-ttu-id="d857a-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d857a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d857a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d857a-139">Response</span></span>

<span data-ttu-id="d857a-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens [usados](../resources/insights-used.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d857a-140">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d857a-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d857a-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d857a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d857a-142">Request</span></span>

<span data-ttu-id="d857a-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d857a-143">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="d857a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d857a-144">Response</span></span>

<span data-ttu-id="d857a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d857a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```


