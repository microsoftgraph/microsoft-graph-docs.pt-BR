---
title: Listar usados
description: Visão calculada que retorna a lista de arquivos usados com um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 3bd97a9c727a88cd4677de359880c79ed8a85e39
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39843858"
---
# <a name="list-used"></a><span data-ttu-id="ede0e-103">Listar usados</span><span class="sxs-lookup"><span data-stu-id="ede0e-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ede0e-104">Informações calculadas que incluem uma lista de documentos modificados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="ede0e-104">Calculated insight that includes a list of documents the user has modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="ede0e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ede0e-105">Permissions</span></span>
<span data-ttu-id="ede0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ede0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ede0e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ede0e-108">Permission type</span></span>      | <span data-ttu-id="ede0e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ede0e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ede0e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ede0e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ede0e-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ede0e-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ede0e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ede0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ede0e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ede0e-113">Not supported.</span></span>    |
|<span data-ttu-id="ede0e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ede0e-114">Application</span></span> | <span data-ttu-id="ede0e-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ede0e-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ede0e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ede0e-116">HTTP request</span></span>
<span data-ttu-id="ede0e-117">Obter uma lista de documentos que o usuário conectado modificou:</span><span class="sxs-lookup"><span data-stu-id="ede0e-117">Get a list of documents that the signed-in user has modified:</span></span>

```http
GET /me/insights/used
```

<span data-ttu-id="ede0e-118">Obtém uma lista de documentos que o usuário especificado modificou.</span><span class="sxs-lookup"><span data-stu-id="ede0e-118">Get a list of documents that the specified user has modified.</span></span>

><span data-ttu-id="ede0e-119">**Observação**: a solicitação de documentos **usados** por outro usuário retorna resultados classificados por **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="ede0e-119">**Note**: Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="ede0e-120">**lastAccessedDateTime** é então definido como **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="ede0e-120">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>
```http
GET /users/{id | userPrincipalName}/insights/used
```

<span data-ttu-id="ede0e-121">Expanda o recurso mencionado por uma percepção **usada** :</span><span class="sxs-lookup"><span data-stu-id="ede0e-121">Expand the resource referenced by a **used** insight:</span></span>

```http
GET /me/insights/used/{id}/resource
GET /users/{id | userPrincipalName}/insights/used/{id}/resource
```


## <a name="optional-query-parameters"></a><span data-ttu-id="ede0e-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ede0e-122">Optional query parameters</span></span>
<span data-ttu-id="ede0e-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ede0e-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ede0e-124">Você pode usar o `$filter` parâmetro de consulta para filtrar itens usados.</span><span class="sxs-lookup"><span data-stu-id="ede0e-124">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="ede0e-125">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="ede0e-125">For example, based on **type**:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="ede0e-126">Ou com base no **ContainerType**:</span><span class="sxs-lookup"><span data-stu-id="ede0e-126">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="ede0e-127">Confira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="ede0e-127">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="ede0e-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ede0e-128">Request headers</span></span>
| <span data-ttu-id="ede0e-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ede0e-129">Header</span></span>       |  <span data-ttu-id="ede0e-130">Valor</span><span class="sxs-lookup"><span data-stu-id="ede0e-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="ede0e-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ede0e-131">Authorization</span></span>  | <span data-ttu-id="ede0e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ede0e-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ede0e-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ede0e-134">Accept</span></span>  | <span data-ttu-id="ede0e-135">application/json</span><span class="sxs-lookup"><span data-stu-id="ede0e-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ede0e-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ede0e-136">Request body</span></span>
<span data-ttu-id="ede0e-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ede0e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ede0e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ede0e-138">Response</span></span>

<span data-ttu-id="ede0e-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens [usados](../resources/insights-used.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ede0e-139">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ede0e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ede0e-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ede0e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ede0e-141">Request</span></span>

<span data-ttu-id="ede0e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ede0e-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="ede0e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ede0e-143">Response</span></span>

<span data-ttu-id="ede0e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ede0e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

