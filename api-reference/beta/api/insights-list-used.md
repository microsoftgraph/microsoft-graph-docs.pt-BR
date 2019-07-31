---
title: Listar usados
description: Informações calculadas que retornam a lista de arquivos usados com um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 31115a845c3b5af80aaba700e55e0ede05d922b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953070"
---
# <a name="list-used"></a><span data-ttu-id="949d2-103">Listar usados</span><span class="sxs-lookup"><span data-stu-id="949d2-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="949d2-104">Informações calculadas que retornam a lista de arquivos usados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="949d2-104">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="949d2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="949d2-105">Permissions</span></span>
<span data-ttu-id="949d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="949d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="949d2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="949d2-108">Permission type</span></span>      | <span data-ttu-id="949d2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="949d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="949d2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="949d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="949d2-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="949d2-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="949d2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="949d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="949d2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="949d2-113">Not supported.</span></span>    |
|<span data-ttu-id="949d2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="949d2-114">Application</span></span> | <span data-ttu-id="949d2-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="949d2-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="949d2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="949d2-116">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="949d2-117">Solicitar que os documentos usados de outros usuários retornem resultados classificados por "lastModifiedDateTime" e "lastAccessedDateTime" está definido como "lastModifiedDateTime".</span><span class="sxs-lookup"><span data-stu-id="949d2-117">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/{id | userPrincipalName}/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="949d2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="949d2-118">Optional query parameters</span></span>
<span data-ttu-id="949d2-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="949d2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="949d2-120">Você pode usar o `$filter` parâmetro de consulta para filtrar itens usados.</span><span class="sxs-lookup"><span data-stu-id="949d2-120">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="949d2-121">Por exemplo, com base no tipo:</span><span class="sxs-lookup"><span data-stu-id="949d2-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="949d2-122">Ou com base no tipo de contêiner:</span><span class="sxs-lookup"><span data-stu-id="949d2-122">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="949d2-123">Confira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="949d2-123">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="949d2-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="949d2-124">Request headers</span></span>
| <span data-ttu-id="949d2-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="949d2-125">Header</span></span>       |  <span data-ttu-id="949d2-126">Valor</span><span class="sxs-lookup"><span data-stu-id="949d2-126">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="949d2-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="949d2-127">Authorization</span></span>  | <span data-ttu-id="949d2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="949d2-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="949d2-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="949d2-130">Accept</span></span>  | <span data-ttu-id="949d2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="949d2-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="949d2-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="949d2-132">Request body</span></span>
<span data-ttu-id="949d2-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="949d2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="949d2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="949d2-134">Response</span></span>

<span data-ttu-id="949d2-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens [usados](../resources/insights-used.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="949d2-135">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="949d2-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="949d2-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="949d2-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="949d2-137">Request</span></span>

<span data-ttu-id="949d2-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="949d2-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="949d2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="949d2-139">Response</span></span>

<span data-ttu-id="949d2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="949d2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

### <a name="expanding-resource"></a><span data-ttu-id="949d2-143">Expandindo recurso</span><span class="sxs-lookup"><span data-stu-id="949d2-143">Expanding resource</span></span>
<span data-ttu-id="949d2-144">O recurso mencionado por uma visão usada pode ser expandido.</span><span class="sxs-lookup"><span data-stu-id="949d2-144">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
