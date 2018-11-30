---
title: Lista usada
description: Percepção calculada que retorna a lista de arquivos usados com um usuário.
ms.openlocfilehash: a9e5390e38e4e697f55676304edb4544e4c2ded5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037610"
---
# <a name="list-used"></a><span data-ttu-id="1afd6-103">Lista usada</span><span class="sxs-lookup"><span data-stu-id="1afd6-103">List used</span></span>

> <span data-ttu-id="1afd6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1afd6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1afd6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1afd6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1afd6-106">Percepção calculada que retorna a lista de arquivos usados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="1afd6-106">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1afd6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1afd6-107">Permissions</span></span>
<span data-ttu-id="1afd6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1afd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1afd6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1afd6-110">Permission type</span></span>      | <span data-ttu-id="1afd6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1afd6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1afd6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1afd6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1afd6-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afd6-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1afd6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1afd6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1afd6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1afd6-115">Not supported.</span></span>    |
|<span data-ttu-id="1afd6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1afd6-116">Application</span></span> | <span data-ttu-id="1afd6-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afd6-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1afd6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1afd6-118">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="1afd6-119">Solicitando documentos usados ela retorna os resultados do outro usuário classificados por 'lastModifiedDateTime' e 'lastAccessedDateTime' for definido como 'lastModifiedDateTime'.</span><span class="sxs-lookup"><span data-stu-id="1afd6-119">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1afd6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1afd6-120">Optional query parameters</span></span>
<span data-ttu-id="1afd6-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1afd6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1afd6-122">Você pode usar o `$filter` consulta parâmetro aos itens de filtro usado.</span><span class="sxs-lookup"><span data-stu-id="1afd6-122">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="1afd6-123">Por exemplo, com base no tipo:</span><span class="sxs-lookup"><span data-stu-id="1afd6-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="1afd6-124">Ou com base no tipo de contêiner:</span><span class="sxs-lookup"><span data-stu-id="1afd6-124">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="1afd6-125">Consulte os tipos de contêiner e os tipos que você pode filtrar por em [resourceVisualization](../resources/insights-resourcevisualization.md)a disponíveis.</span><span class="sxs-lookup"><span data-stu-id="1afd6-125">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="1afd6-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1afd6-126">Request headers</span></span>
| <span data-ttu-id="1afd6-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1afd6-127">Header</span></span>       |  <span data-ttu-id="1afd6-128">Valor</span><span class="sxs-lookup"><span data-stu-id="1afd6-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="1afd6-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="1afd6-129">Authorization</span></span>  | <span data-ttu-id="1afd6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1afd6-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1afd6-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1afd6-132">Accept</span></span>  | <span data-ttu-id="1afd6-133">application/json</span><span class="sxs-lookup"><span data-stu-id="1afd6-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1afd6-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1afd6-134">Request body</span></span>
<span data-ttu-id="1afd6-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1afd6-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1afd6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1afd6-136">Response</span></span>

<span data-ttu-id="1afd6-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de itens [utilizados](../resources/insights-used.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1afd6-137">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1afd6-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1afd6-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1afd6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1afd6-139">Request</span></span>

<span data-ttu-id="1afd6-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1afd6-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="1afd6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1afd6-141">Response</span></span>

<span data-ttu-id="1afd6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1afd6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

### <a name="expanding-resource"></a><span data-ttu-id="1afd6-145">A expansão de recurso</span><span class="sxs-lookup"><span data-stu-id="1afd6-145">Expanding resource</span></span>
<span data-ttu-id="1afd6-146">O recurso referenciado por um insight usado pode ser expandido.</span><span class="sxs-lookup"><span data-stu-id="1afd6-146">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
